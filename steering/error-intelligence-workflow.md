# Error Intelligence Workflow

## When to Use This Workflow

Activate when user:
- Provides an error message or error code
- Asks to "look up" or "search for" an error
- Mentions debugging or troubleshooting
- Shares stack traces or error logs

---

## Multi-Phase Error Intelligence Protocol

### Phase 1: Error Classification

**Immediate Actions:**
1. Extract error code/message
2. Identify framework/library
3. Determine error type:
   - Syntax error
   - Runtime error
   - Configuration error
   - Network error
   - Authentication error
   - Database error

4. Assess severity:
   - Critical (blocks functionality)
   - High (major feature broken)
   - Medium (workaround available)
   - Low (minor issue)

**Output Format:**
```
ERROR CLASSIFICATION
===================
Error Code: [code]
Error Message: [message]
Framework: [name] v[version]
Type: [error type]
Severity: [level]
```

---

### Phase 2: Structured Search Strategy

**Search Sequence:**

1. **Official Documentation Search**
   ```
   Query: "[framework] [error code] official documentation"
   Priority: Highest
   ```

2. **GitHub Issues Search**
   ```
   Query: "[framework] [error code] is:issue"
   Filter: Look for closed issues with solutions
   Priority: High
   ```

3. **Stack Overflow Search**
   ```
   Query: "[framework] [error code] [accepted:yes]"
   Filter: Accepted answers only
   Priority: High
   ```

4. **Community Forums Search**
   ```
   Query: "[framework] [error code] solution"
   Priority: Medium
   ```

**Search Best Practices:**
- Use exact error string in quotes
- Include framework version when known
- Add "solved" or "fixed" to queries
- Check publication dates (prefer recent)

---

### Phase 3: Solution Extraction & Validation

**For Each Source Found:**

1. **Extract Information:**
   - Root cause explanation
   - Step-by-step solution
   - Code examples
   - Version compatibility
   - Side effects or warnings

2. **Validate Solution:**
   - Check if solution is for correct version
   - Verify solution is still valid (not outdated)
   - Confirm no breaking changes since posted
   - Check for community verification (upvotes, acceptance)

3. **Assess Quality:**
   - Official source: ⭐⭐⭐⭐⭐
   - Maintainer response: ⭐⭐⭐⭐
   - Accepted answer: ⭐⭐⭐⭐
   - Community solution: ⭐⭐⭐
   - Unverified: ⭐⭐

---

### Phase 4: Structured Output Generation

**Always Provide:**

```
ERROR INTELLIGENCE REPORT
========================

ERROR DETAILS
-------------
Code: [error code]
Message: [full error message]
Framework: [name] v[version]
Severity: [Critical/High/Medium/Low]

ROOT CAUSE
----------
[Clear explanation of why this error occurs]

COMMON TRIGGERS
---------------
1. [Trigger 1 - most common]
2. [Trigger 2]
3. [Trigger 3]

VERIFIED SOLUTIONS
------------------

Solution 1: [Primary Solution]
Source: [URL]
Verified: [date/version]
Quality: ⭐⭐⭐⭐⭐

Steps:
1. [Step 1 with code if applicable]
2. [Step 2]
3. [Step 3]

Expected Result: [what should happen]

Solution 2: [Alternative Solution]
Source: [URL]
Verified: [date/version]
Quality: ⭐⭐⭐⭐

Steps:
1. [Step 1]
2. [Step 2]

When to use: [conditions for this alternative]

PREVENTION STRATEGIES
--------------------
- [Strategy 1 to avoid this error]
- [Strategy 2]
- [Strategy 3]

VERSION COMPATIBILITY
--------------------
- Affected versions: [version range]
- Fixed in: [version if applicable]
- Workaround needed for: [versions]

RELATED ISSUES
--------------
- [Related error 1]: [brief description]
- [Related error 2]: [brief description]

TESTING VERIFICATION
-------------------
To verify the fix works:
1. [Verification step 1]
2. [Verification step 2]
3. [Expected outcome]

SOURCES
-------
- [Official docs URL]
- [GitHub issue URL]
- [Stack Overflow URL]
- [Additional source URL]

CONFIDENCE LEVEL
---------------
[High/Medium/Low] - Based on source quality and verification
```

---

## Special Cases

### Case 1: No Official Documentation Found

**Response:**
```
⚠️ LIMITED DOCUMENTATION

Official documentation for this error was not found.

Sources checked:
- Official docs: Not found
- GitHub issues: [X found]
- Stack Overflow: [X found]

Proceeding with community-verified solutions.
Confidence Level: Medium

Recommendation: Test thoroughly in development before production.
```

### Case 2: Version-Specific Error

**Response:**
```
⚠️ VERSION-SPECIFIC ERROR

This error is specific to [framework] v[version].

Version Context:
- Your version: [version]
- Error introduced in: [version]
- Fixed in: [version if applicable]

Recommendation:
[Upgrade/Downgrade/Workaround] based on your situation.
```

### Case 3: Breaking Change Error

**Response:**
```
⚠️ BREAKING CHANGE DETECTED

This error is caused by a breaking change in [framework] v[version].

Breaking Change:
[Description of what changed]

Migration Required:
[What needs to be updated]

Migration Guide: [URL if available]
```

---

## Error Pattern Recognition

### Common Error Patterns

**Authentication Errors:**
- Pattern: `auth/`, `401`, `unauthorized`
- Common causes: Invalid credentials, expired tokens, missing permissions
- First check: Credentials, token expiry, API keys

**Database Errors:**
- Pattern: `ECONNREFUSED`, `connection`, `database`
- Common causes: Database not running, wrong connection string, network issues
- First check: Database status, connection string, network connectivity

**Configuration Errors:**
- Pattern: `config`, `environment`, `missing`
- Common causes: Missing env variables, wrong config format, missing files
- First check: .env file, config files, environment setup

**Dependency Errors:**
- Pattern: `module not found`, `cannot find`, `ENOENT`
- Common causes: Missing dependencies, wrong import path, version mismatch
- First check: package.json, node_modules, import statements

---

## Quality Assurance Checklist

Before providing error intelligence:

- [ ] Error code/message extracted correctly
- [ ] Framework and version identified
- [ ] Multiple sources consulted (minimum 2)
- [ ] Solutions verified for correct version
- [ ] Root cause clearly explained
- [ ] Step-by-step solutions provided
- [ ] Prevention strategies included
- [ ] Sources cited with URLs
- [ ] Confidence level assessed
- [ ] Testing verification steps included

---

## Example: Complete Error Intelligence

**User Input:**
```
"Look up Firebase auth/invalid-credential error"
```

**Kiro Response:**
```
ERROR INTELLIGENCE REPORT
========================

ERROR DETAILS
-------------
Code: auth/invalid-credential
Message: The supplied auth credential is malformed or has expired
Framework: Firebase Authentication v10
Severity: Medium

ROOT CAUSE
----------
This error occurs when Firebase receives credentials that are either:
1. Incorrectly formatted
2. Expired or invalid
3. Don't match any existing user account

This is EXPECTED BEHAVIOR for security - Firebase doesn't reveal whether 
an email exists to prevent account enumeration attacks.

COMMON TRIGGERS
---------------
1. User entered wrong email or password (most common)
2. Account doesn't exist with provided credentials
3. OAuth token has expired
4. Credential object is malformed
5. Account exists but with different auth provider

VERIFIED SOLUTIONS
------------------

Solution 1: Verify User Input
Source: https://firebase.google.com/docs/auth/admin/errors
Verified: 2024
Quality: ⭐⭐⭐⭐⭐

Steps:
1. Validate email format before submission
2. Check password meets requirements
3. Implement proper error handling:

```javascript
try {
  await signInWithEmailAndPassword(auth, email, password);
} catch (error) {
  if (error.code === 'auth/invalid-credential') {
    // Show generic message for security
    setError('Invalid email or password');
  }
}
```

Expected Result: User sees friendly error message

Solution 2: Check Account Exists
Source: https://stackoverflow.com/questions/57010980
Verified: 2024
Quality: ⭐⭐⭐⭐

Steps:
1. Verify account was created
2. Check if account uses different provider (Google, Facebook)
3. Provide "Forgot Password" option

When to use: When user reports they "can't log in"

PREVENTION STRATEGIES
--------------------
- Validate input format before submission
- Implement "Forgot Password" flow
- Show which auth providers are available
- Don't reveal whether email exists (security)
- Provide clear error messages
- Add rate limiting to prevent brute force

VERSION COMPATIBILITY
--------------------
- Affected versions: All Firebase Auth versions
- Behavior: Consistent across versions
- Note: This is a security feature, not a bug

RELATED ISSUES
--------------
- auth/user-not-found: Deprecated, now returns invalid-credential
- auth/wrong-password: Deprecated, now returns invalid-credential

TESTING VERIFICATION
-------------------
To verify the fix works:
1. Test with valid credentials → Should succeed
2. Test with invalid credentials → Should show error
3. Test with non-existent email → Should show same error
4. Verify error message is user-friendly

SOURCES
-------
- https://firebase.google.com/docs/auth/admin/errors
- https://stackoverflow.com/questions/57010980
- https://github.com/firebase/firebase-js-sdk/issues/...

CONFIDENCE LEVEL
---------------
High - Based on official documentation and verified community sources
```

---

## Advanced: Error Pattern Database

**Build knowledge of common errors:**

When encountering errors repeatedly:
1. Note the pattern
2. Document common solutions
3. Build error-solution mapping
4. Improve future responses

**Example Pattern:**
```
Pattern: "hydration mismatch" in Next.js
Common Cause: Server/client HTML mismatch
Quick Solution: Check for browser-only APIs, date formatting, random values
Prevention: Use useEffect for client-only code
```

---

This workflow ensures every error gets professional-grade intelligence with verified solutions and clear implementation guidance.
