# Migration Planning Workflow

## When to Use This Workflow

Activate when user:
- Plans framework/library upgrades
- Asks about migration paths
- Needs breaking change analysis
- Requests migration guides
- Plans major version upgrades

---

## Professional Migration Planning Protocol

### Phase 1: Migration Scope Assessment

**Initial Analysis:**

1. **Identify Migration Type**
   - Framework upgrade (e.g., Next.js 14 → 15)
   - Library upgrade (e.g., React 18 → 19)
   - Language upgrade (e.g., TypeScript 4 → 5)
   - Platform migration (e.g., Pages Router → App Router)
   - Database migration (e.g., Firebase v9 → v10)

2. **Version Gap Analysis**
   ```
   MIGRATION SCOPE
   ==============
   From: [package] v[current]
   To: [package] v[target]
   Version gap: [number] major versions
   Release span: [time period]
   ```

3. **Impact Assessment**
   ```
   IMPACT LEVEL: [Low/Medium/High/Critical]
   
   Factors:
   - Breaking changes: [number]
   - Deprecated APIs: [number]
   - New required dependencies: [number]
   - Config changes: [number]
   - Code changes: [estimated scope]
   ```

---

### Phase 2: Breaking Change Analysis

**Comprehensive Breaking Change Review:**

1. **Fetch All Release Notes**
   - Between current and target versions
   - Focus on BREAKING CHANGES sections
   - Note deprecation warnings
   - Identify removed features

2. **Categorize Breaking Changes**
   ```
   BREAKING CHANGES BY CATEGORY
   ============================
   
   API Changes:
   - [Change 1]: [old API] → [new API]
   - [Change 2]: [old API] → [new API]
   
   Configuration Changes:
   - [Change 1]: [old config] → [new config]
   - [Change 2]: [old config] → [new config]
   
   Behavior Changes:
   - [Change 1]: [old behavior] → [new behavior]
   - [Change 2]: [old behavior] → [new behavior]
   
   Removed Features:
   - [Feature 1]: Removed in v[version]
   - [Feature 2]: Removed in v[version]
   
   Dependency Changes:
   - [Dep 1]: Now requires v[version]
   - [Dep 2]: No longer compatible
   ```

3. **Assess Impact of Each Change**
   ```
   CHANGE IMPACT ANALYSIS
   =====================
   
   Change: [description]
   Impact: [High/Medium/Low]
   Affects: [what code/files]
   Effort: [hours/days]
   Risk: [High/Medium/Low]
   Migration: [how to update]
   ```

---

### Phase 3: Migration Strategy Development

**Create Structured Migration Plan:**

1. **Migration Approach**
   ```
   MIGRATION STRATEGY
   =================
   
   Approach: [Big Bang / Incremental / Parallel]
   
   Big Bang:
   - Upgrade everything at once
   - Pros: Faster, cleaner
   - Cons: Higher risk, more downtime
   - Best for: Small projects, low complexity
   
   Incremental:
   - Upgrade in phases
   - Pros: Lower risk, easier rollback
   - Cons: Longer timeline, temporary complexity
   - Best for: Large projects, high complexity
   
   Parallel:
   - Run old and new versions side-by-side
   - Pros: Zero downtime, gradual migration
   - Cons: Most complex, resource intensive
   - Best for: Critical systems, zero-downtime requirement
   
   RECOMMENDED: [approach] because [rationale]
   ```

2. **Phase Breakdown**
   ```
   MIGRATION PHASES
   ===============
   
   Phase 1: Preparation (Week 1)
   - [ ] Backup current codebase
   - [ ] Document current state
   - [ ] Set up test environment
   - [ ] Review migration guides
   - [ ] Identify all affected files
   
   Phase 2: Dependencies (Week 1-2)
   - [ ] Update package.json
   - [ ] Resolve dependency conflicts
   - [ ] Update peer dependencies
   - [ ] Test dependency compatibility
   
   Phase 3: Code Migration (Week 2-3)
   - [ ] Update API calls
   - [ ] Migrate deprecated features
   - [ ] Update configurations
   - [ ] Fix breaking changes
   - [ ] Update types/interfaces
   
   Phase 4: Testing (Week 3-4)
   - [ ] Unit tests
   - [ ] Integration tests
   - [ ] E2E tests
   - [ ] Performance testing
   - [ ] Security testing
   
   Phase 5: Deployment (Week 4)
   - [ ] Deploy to staging
   - [ ] Smoke testing
   - [ ] Deploy to production
   - [ ] Monitor for issues
   - [ ] Document changes
   ```

3. **Risk Mitigation**
   ```
   RISK MITIGATION PLAN
   ===================
   
   Risk 1: [Description]
   Probability: [High/Medium/Low]
   Impact: [High/Medium/Low]
   Mitigation:
   - [Strategy 1]
   - [Strategy 2]
   Contingency: [backup plan]
   
   Risk 2: [Description]
   Probability: [High/Medium/Low]
   Impact: [High/Medium/Low]
   Mitigation:
   - [Strategy 1]
   - [Strategy 2]
   Contingency: [backup plan]
   ```

---

### Phase 4: Implementation Guidance

**Detailed Migration Instructions:**

1. **Pre-Migration Checklist**
   ```
   PRE-MIGRATION CHECKLIST
   ======================
   
   Code Preparation:
   - [ ] Create feature branch
   - [ ] Backup database
   - [ ] Document current behavior
   - [ ] Freeze new features
   - [ ] Notify team/stakeholders
   
   Environment Setup:
   - [ ] Set up test environment
   - [ ] Configure CI/CD for new version
   - [ ] Prepare rollback procedure
   - [ ] Set up monitoring
   
   Documentation:
   - [ ] Review official migration guide
   - [ ] Document custom code changes needed
   - [ ] Create testing checklist
   - [ ] Prepare deployment runbook
   ```

2. **Step-by-Step Migration**
   ```
   MIGRATION STEPS
   ==============
   
   Step 1: Update Dependencies
   ```bash
   # Update package.json
   npm install [package]@[version]
   
   # Or with specific version
   npm install [package]@latest
   
   # Check for peer dependency warnings
   npm ls
   ```
   
   Step 2: Update Configuration
   ```[language]
   // Old configuration
   [old config code]
   
   // New configuration
   [new config code]
   ```
   
   Step 3: Migrate API Calls
   ```[language]
   // Before
   [old API usage]
   
   // After
   [new API usage]
   ```
   
   Step 4: Update Types (if TypeScript)
   ```typescript
   // Old types
   [old type definitions]
   
   // New types
   [new type definitions]
   ```
   
   Step 5: Fix Breaking Changes
   [Detailed instructions for each breaking change]
   
   Step 6: Run Tests
   ```bash
   npm test
   npm run test:integration
   npm run test:e2e
   ```
   
   Step 7: Verify Functionality
   - [ ] [Feature 1] works correctly
   - [ ] [Feature 2] works correctly
   - [ ] [Feature 3] works correctly
   ```

3. **Testing Strategy**
   ```
   TESTING STRATEGY
   ===============
   
   Unit Tests:
   - Test all modified functions
   - Test edge cases
   - Test error handling
   - Target: 100% coverage of changed code
   
   Integration Tests:
   - Test API integrations
   - Test database operations
   - Test third-party services
   - Test authentication flows
   
   E2E Tests:
   - Test critical user flows
   - Test all major features
   - Test cross-browser compatibility
   - Test mobile responsiveness
   
   Performance Tests:
   - Benchmark before migration
   - Benchmark after migration
   - Compare metrics
   - Identify regressions
   
   Security Tests:
   - Run security audit
   - Check for vulnerabilities
   - Test authentication
   - Test authorization
   ```

---

## Complete Migration Plan Format

```
PROFESSIONAL MIGRATION PLAN
===========================

EXECUTIVE SUMMARY
----------------
Migration: [package] v[from] → v[to]
Complexity: [Low/Medium/High]
Estimated Duration: [time]
Risk Level: [Low/Medium/High]
Recommended Approach: [approach]

PROJECT OVERVIEW
---------------
Current Version: v[version]
Target Version: v[version]
Version Gap: [number] major versions
Release Span: [time period]
Last Updated: [date]

BREAKING CHANGES SUMMARY
-----------------------
Total Breaking Changes: [number]
- High Impact: [number]
- Medium Impact: [number]
- Low Impact: [number]

Key Changes:
1. [Change 1] - Impact: [level]
2. [Change 2] - Impact: [level]
3. [Change 3] - Impact: [level]

IMPACT ASSESSMENT
----------------
Code Changes Required:
- Files affected: [number]
- Lines of code: [estimate]
- New dependencies: [number]
- Removed dependencies: [number]

Effort Estimation:
- Development: [hours/days]
- Testing: [hours/days]
- Documentation: [hours/days]
- Total: [hours/days]

Team Resources:
- Developers needed: [number]
- QA resources: [number]
- DevOps support: [yes/no]

MIGRATION STRATEGY
-----------------
Approach: [Big Bang/Incremental/Parallel]
Rationale: [why this approach]

Timeline:
- Phase 1: [dates] - [activities]
- Phase 2: [dates] - [activities]
- Phase 3: [dates] - [activities]
- Phase 4: [dates] - [activities]

DETAILED MIGRATION STEPS
------------------------
[Step-by-step instructions with code examples]

TESTING PLAN
-----------
[Comprehensive testing strategy]

RISK ANALYSIS
------------
[Identified risks with mitigation strategies]

ROLLBACK PLAN
------------
If migration fails:
1. [Rollback step 1]
2. [Rollback step 2]
3. [Rollback step 3]

Rollback triggers:
- [Trigger 1]
- [Trigger 2]

DEPLOYMENT STRATEGY
------------------
Environment Sequence:
1. Development → [date]
2. Staging → [date]
3. Production → [date]

Deployment Steps:
1. [Step 1]
2. [Step 2]
3. [Step 3]

Monitoring:
- [Metric 1]
- [Metric 2]
- [Metric 3]

POST-MIGRATION
-------------
Verification Checklist:
- [ ] All tests passing
- [ ] Performance metrics acceptable
- [ ] No critical errors
- [ ] User acceptance testing complete

Documentation Updates:
- [ ] Update README
- [ ] Update API docs
- [ ] Update deployment docs
- [ ] Update team wiki

Team Communication:
- [ ] Notify stakeholders
- [ ] Update team
- [ ] Document lessons learned

SOURCES & REFERENCES
-------------------
- Official migration guide: [URL]
- Release notes: [URL]
- Community discussions: [URL]
- Related issues: [URL]

APPROVAL & SIGN-OFF
------------------
Prepared by: [name]
Reviewed by: [name]
Approved by: [name]
Date: [date]
```

---

## Quality Assurance Checklist

Before providing migration plan:

- [ ] All breaking changes identified
- [ ] Migration complexity assessed
- [ ] Timeline estimated
- [ ] Risks identified and mitigated
- [ ] Testing strategy defined
- [ ] Rollback plan included
- [ ] Step-by-step instructions provided
- [ ] Code examples included
- [ ] Sources cited
- [ ] Professional format used

---

## Special Cases

### Case 1: Multi-Package Migration

```
⚠️ MULTI-PACKAGE MIGRATION

This migration affects multiple packages:
- [Package 1]: v[from] → v[to]
- [Package 2]: v[from] → v[to]
- [Package 3]: v[from] → v[to]

DEPENDENCY CHAIN:
[Package 1] → [Package 2] → [Package 3]

RECOMMENDED ORDER:
1. Upgrade [Package 3] first (no dependencies)
2. Then upgrade [Package 2] (depends on 3)
3. Finally upgrade [Package 1] (depends on 2)

Complexity: High
Risk: High
Recommendation: Incremental approach with thorough testing
```

### Case 2: Zero-Downtime Migration

```
🎯 ZERO-DOWNTIME REQUIREMENT

Strategy: Blue-Green Deployment

Approach:
1. Set up parallel environment (Green)
2. Deploy new version to Green
3. Test Green environment
4. Switch traffic to Green
5. Keep Blue as fallback
6. Monitor for issues
7. Decommission Blue after stability confirmed

Requirements:
- Load balancer configuration
- Database compatibility
- Session management
- Monitoring setup

Timeline: [extended due to parallel setup]
```

### Case 3: Breaking Change Workaround

```
⚠️ BREAKING CHANGE WORKAROUND AVAILABLE

Breaking Change: [description]
Official Migration: [complex/time-consuming]

WORKAROUND AVAILABLE:
[Description of workaround]

Pros:
- Faster implementation
- Less code changes
- Lower risk

Cons:
- Not official solution
- May need future update
- Potential limitations

Recommendation: [use workaround/follow official] because [rationale]
```

---

This workflow ensures professional-grade migration planning with comprehensive risk assessment and clear implementation guidance.
