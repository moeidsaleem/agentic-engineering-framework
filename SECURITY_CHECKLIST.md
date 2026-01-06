---
layout: default
title: Security Checklist
description: Comprehensive security checklist for AI engineering - authentication, data protection, input validation, API security, and infrastructure security best practices
keywords: AI security checklist, engineering security, authentication security, data protection, API security, security best practices
---

# Security Checklist

**Author:** Moeid Saleem Khan  
**Version:** 2.0

A comprehensive security checklist to review before marking any work complete.

---

## Authentication & Authorization

- [ ] Authentication implemented correctly
- [ ] Authorization checks in place
- [ ] Role-based access control (if applicable)
- [ ] Session management secure
- [ ] Token expiration handled
- [ ] Password policies enforced
- [ ] Multi-factor authentication (if required)

---

## Data Protection

- [ ] Sensitive data encrypted at rest
- [ ] Sensitive data encrypted in transit
- [ ] Passwords hashed (bcrypt, argon2, etc.)
- [ ] API keys stored securely (not hardcoded)
- [ ] Secrets in environment variables
- [ ] No credentials in code or logs
- [ ] PII handled according to regulations

---

## Input Validation

- [ ] All user inputs validated
- [ ] Input sanitization in place
- [ ] SQL injection prevented (parameterized queries)
- [ ] XSS prevention (output encoding)
- [ ] CSRF protection
- [ ] File upload validation
- [ ] Rate limiting on inputs

---

## API Security

- [ ] API endpoints authenticated
- [ ] API endpoints authorized
- [ ] Rate limiting implemented
- [ ] CORS configured correctly
- [ ] API versioning handled
- [ ] Error messages don't leak information
- [ ] Request size limits

---

## Infrastructure Security

- [ ] HTTPS enforced
- [ ] Security headers configured
- [ ] Dependencies up to date
- [ ] Known vulnerabilities patched
- [ ] Firewall rules appropriate
- [ ] Access logs enabled
- [ ] Monitoring and alerting configured

---

## Code Security

- [ ] No hardcoded secrets
- [ ] No debug code in production
- [ ] Error handling doesn't expose internals
- [ ] Logging doesn't include sensitive data
- [ ] Dependencies scanned for vulnerabilities
- [ ] Code review completed
- [ ] Security tests included

---

## Database Security

- [ ] Database credentials secure
- [ ] Connection strings encrypted
- [ ] SQL injection prevented
- [ ] Database access restricted
- [ ] Backups encrypted
- [ ] Audit logging enabled
- [ ] Row-level security (if applicable)

---

## Third-Party Integrations

- [ ] API keys stored securely
- [ ] OAuth flows implemented correctly
- [ ] Webhook signatures verified
- [ ] Third-party dependencies vetted
- [ ] External API calls authenticated
- [ ] Error handling for external failures

---

## Compliance & Privacy

- [ ] GDPR compliance (if applicable)
- [ ] Data retention policies followed
- [ ] User consent obtained (if required)
- [ ] Privacy policy updated
- [ ] Data deletion implemented
- [ ] Audit trails maintained

---

## Deployment Security

- [ ] Production secrets not in code
- [ ] Environment variables secured
- [ ] Deployment keys rotated
- [ ] CI/CD pipelines secure
- [ ] Container images scanned
- [ ] Infrastructure as code reviewed

---

## Monitoring & Incident Response

- [ ] Security events logged
- [ ] Alerts configured for suspicious activity
- [ ] Incident response plan documented
- [ ] Security monitoring in place
- [ ] Regular security audits scheduled

---

## Quick Security Review Questions

Before marking work complete, ask:

1. **Are there any secrets exposed?**
   - Check code, logs, configs, commits

2. **Is user input validated?**
   - All inputs sanitized and validated

3. **Are authentication/authorization checks in place?**
   - Protected endpoints verified

4. **Is sensitive data protected?**
   - Encrypted, hashed, or properly secured

5. **Are dependencies secure?**
   - No known vulnerabilities

6. **Is error handling secure?**
   - No information leakage

7. **Is logging secure?**
   - No sensitive data in logs

---

## Security Anti-Patterns to Avoid

### ❌ Hardcoding Secrets
```javascript
// BAD
const API_KEY = "sk_live_1234567890";

// GOOD
const API_KEY = process.env.API_KEY;
```

### ❌ Exposing Internal Errors
```javascript
// BAD
res.status(500).json({ error: err.stack });

// GOOD
res.status(500).json({ error: "Internal server error" });
// Log full error server-side
```

### ❌ Not Validating Input
```javascript
// BAD
const user = await db.query(`SELECT * FROM users WHERE id = ${req.params.id}`);

// GOOD
const user = await db.query('SELECT * FROM users WHERE id = $1', [req.params.id]);
```

### ❌ Storing Passwords in Plain Text
```javascript
// BAD
await db.query('INSERT INTO users (email, password) VALUES ($1, $2)', [email, password]);

// GOOD
const hashedPassword = await bcrypt.hash(password, 10);
await db.query('INSERT INTO users (email, password) VALUES ($1, $2)', [email, hashedPassword]);
```

---

## Security Resources

- OWASP Top 10
- CWE Top 25
- Security best practices for your stack
- Framework-specific security guides

---

## When to Escalate

Escalate security concerns when:
- Unclear security requirements
- Multiple valid security approaches
- High-risk changes (authentication, payment processing)
- Compliance requirements unclear
- Security vs. usability trade-offs

---

**Remember: Security is not optional. Review this checklist for every change that touches authentication, authorization, data handling, or external integrations.**

