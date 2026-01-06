# Example: Build Workflow in Action

This is a real-world example of how to use the build workflow.

---

## Scenario

**Mission:** Add user authentication with JWT tokens to the API

---

## Phase 1: Discovery

**What the agent does:**

1. **Documentation Review**
   - Checks `docs/`, `README.md` for existing auth patterns
   - Reviews API documentation
   - Finds outdated note: "Auth planned for Q2" (ignores, checks code)

2. **System Architecture Mapping**
   - Discovers existing `middleware/` directory
   - Finds `config/auth.js` with placeholder structure
   - Maps request flow: `router → middleware → controller → service → database`
   - Identifies existing JWT library in `package.json`

3. **Code Pattern Analysis**
   - Studies existing middleware patterns (`middleware/logger.js`, `middleware/validator.js`)
   - Reviews error handling patterns
   - Maps database schema for user table
   - Traces existing API response formats

**Deliverable:**
```
Discovery Report:
- System: Express.js API with middleware pattern
- Existing: JWT library installed, user table exists, middleware structure in place
- Patterns: Middleware exports functions, errors use standard format
- Dependencies: Express, JWT, database connection pool
- Risks: Need to handle token refresh, secure storage
- Status: ✅ No blockers
```

---

## Phase 2: Strategy

**What the agent does:**

1. **Solution Design**
   - Create `middleware/auth.js` following existing pattern
   - Add `routes/auth.js` for login/refresh endpoints
   - Update `services/userService.js` with auth methods
   - Add token validation to protected routes

2. **Risk Assessment**
   - Token expiration handling
   - Secure password hashing (use bcrypt)
   - Rate limiting for login attempts
   - Token storage security

3. **Blocker Check**
   - All clear → Proceed

**Deliverable:**
```
Strategy:
- Approach: Extend existing middleware pattern
- Components:
  - middleware/auth.js (new)
  - routes/auth.js (new)
  - services/userService.js (modify)
  - routes/api.js (modify - add auth middleware)
- Testing: Unit tests for auth middleware, integration tests for login flow
- Risks: Token security, password hashing - mitigated with bcrypt and secure storage
- Status: ✅ Ready to execute
```

---

## Phase 3: Execution

**What the agent does:**

1. **Implementation**
   - Creates `middleware/auth.js` with JWT verification
   - Creates `routes/auth.js` with login/refresh endpoints
   - Updates `services/userService.js` with password hashing
   - Adds auth middleware to protected routes
   - Tests after each component

2. **Continuous Verification**
   - Runs tests after middleware creation → ✅ Pass
   - Runs tests after routes → ✅ Pass
   - Runs integration tests → ⚠️ Token refresh failing
   - Fixes token refresh logic → ✅ All tests pass

3. **Complete Task Chains**
   - Found issue: Token refresh not working
   - Fixed: Updated refresh token validation
   - Verified: All tests pass

**Deliverable:**
```
Execution:
- Created: middleware/auth.js:1-45
- Created: routes/auth.js:1-78
- Modified: services/userService.js:23-45 (added hashPassword, verifyPassword)
- Modified: routes/api.js:12 (added auth middleware)
- Fixed: Token refresh validation in routes/auth.js:45-52
- Tests: All passing
- Status: ✅ Complete
```

---

## Phase 4: Validation

**What the agent does:**

1. **End-to-End Verification**
   - Tests login flow → ✅ Works
   - Tests protected route access → ✅ Works
   - Tests token expiration → ✅ Works
   - Tests refresh token → ✅ Works
   - Checks security: passwords hashed, tokens secure → ✅ Good

2. **Completeness Check**
   - All related issues resolved → ✅
   - Documentation updated → ✅ Updated API docs
   - Temp files cleaned → ✅
   - No debug code → ✅

3. **Final Verification**
   - Tests pass → ✅ 12/12
   - Lint clean → ✅
   - Build successful → ✅
   - System consistent → ✅

**Deliverable:**
```
Validation:
- E2E Tests: All passing
- Security: Passwords hashed, tokens secure
- Documentation: Updated API.md with auth endpoints
- Workspace: Clean
- Final Verdict: ✅ Build complete. System state verified and consistent. Mission accomplished.
```

---

## Key Takeaways

1. **Discovery found existing patterns** - Leveraged middleware structure instead of creating new
2. **Continuous testing** - Caught token refresh issue early
3. **Complete task chain** - Fixed related issue (token refresh) not just main feature
4. **Documentation updated** - Kept docs current with implementation

---

## Full Report Output

```
**Mission:** Add user authentication with JWT tokens to the API

**Phase 1: Discovery**
- Status: ✅
- Findings: Express.js API with middleware pattern. JWT library exists. User table ready. Middleware structure in place.

**Phase 2: Strategy**
- Status: ✅
- Approach: Extend existing middleware pattern
- Components: middleware/auth.js (new), routes/auth.js (new), services/userService.js (modify), routes/api.js (modify)

**Phase 3: Execution**
- Status: ✅
- Changes: Created auth middleware and routes. Updated user service. Fixed token refresh issue.

**Phase 4: Validation**
- Verification Evidence:
  - Tests: 12/12 passing
  - Security: Passwords hashed, tokens secure
  - Documentation: Updated API.md
- Final Verdict:
  - Build complete. System state verified and consistent. Mission accomplished.
```

