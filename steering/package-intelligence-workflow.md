# Package Intelligence Workflow

## When to Use This Workflow

Activate when user:
- Asks about package versions ("What's the latest version of...")
- Requests package comparison ("Compare X vs Y")
- Checks compatibility ("Does X work with Y?")
- Researches breaking changes
- Plans package upgrades

---

## 4-Phase Package Intelligence Protocol

### Phase 1: Version Discovery

**Primary Actions:**

1. **Check Package Registry**
   - npm: `https://registry.npmjs.org/[package-name]`
   - PyPI: `https://pypi.org/pypi/[package-name]/json`
   - Search: "[package-name] latest version"

2. **Extract Version Information:**
   - Latest stable version
   - Latest beta/canary version
   - Previous stable version
   - Release date
   - Release frequency

3. **Verify Official Source:**
   - Official website
   - GitHub repository
   - Package registry
   - Documentation site

**Output Format:**
```
VERSION DISCOVERY
================
Package: [name]
Latest Stable: [version]
Release Date: [date]
Previous Version: [version]
Beta/Canary: [version if available]
Release Frequency: [weekly/monthly/quarterly]
```

---

### Phase 2: Release Analysis

**Comprehensive Release Review:**

1. **Fetch Release Notes**
   - Official changelog
   - GitHub releases
   - Blog announcements
   - Migration guides

2. **Identify Breaking Changes**
   ```
   BREAKING CHANGES:
   - [Change 1]: [Description]
     - Affects: [what code/APIs]
     - Migration: [how to update]
   
   - [Change 2]: [Description]
     - Affects: [what code/APIs]
     - Migration: [how to update]
   ```

3. **Extract New Features**
   ```
   NEW FEATURES:
   - [Feature 1]: [Description]
     - Use case: [when to use]
     - Example: [code example]
   
   - [Feature 2]: [Description]
     - Use case: [when to use]
   ```

4. **Note Deprecations**
   ```
   DEPRECATIONS:
   - [Deprecated API 1]
     - Deprecated in: v[version]
     - Removed in: v[version]
     - Replacement: [new API]
     - Migration: [how to update]
   ```

5. **Check Security Updates**
   ```
   SECURITY UPDATES:
   - [CVE-XXXX-XXXX]: [Description]
     - Severity: [Critical/High/Medium/Low]
     - Affected versions: [range]
     - Fixed in: [version]
   ```

---

### Phase 3: Compatibility Matrix

**Dependency Analysis:**

1. **Peer Dependencies**
   ```
   PEER DEPENDENCIES:
   - [dependency-1]: [version range]
     - Status: ✅ Compatible / ⚠️ Warning / ❌ Incompatible
   
   - [dependency-2]: [version range]
     - Status: ✅ Compatible
   ```

2. **Framework Compatibility**
   ```
   FRAMEWORK COMPATIBILITY:
   - Next.js: v[version range] ✅
   - React: v[version range] ✅
   - Node.js: v[version range] ✅
   - TypeScript: v[version range] ⚠️ (requires config changes)
   ```

3. **Version Conflicts**
   ```
   POTENTIAL CONFLICTS:
   - [package-A] v[version] requires [package-B] v[range]
   - Current [package-B]: v[version]
   - Resolution: [upgrade/downgrade/workaround]
   ```

4. **Ecosystem Impact**
   ```
   ECOSYSTEM IMPACT:
   - Related packages affected: [list]
   - Plugins requiring updates: [list]
   - Tools requiring updates: [list]
   ```

---

### Phase 4: Migration Assessment

**Migration Complexity Analysis:**

1. **Estimate Complexity**
   ```
   MIGRATION COMPLEXITY: [Low/Medium/High]
   
   Factors:
   - Breaking changes: [number]
   - API changes: [number]
   - Config changes: [number]
   - Code changes required: [estimated lines/files]
   ```

2. **Effort Estimation**
   ```
   ESTIMATED EFFORT:
   - Small project: [hours]
   - Medium project: [hours/days]
   - Large project: [days/weeks]
   
   Breakdown:
   - Code updates: [time]
   - Testing: [time]
   - Documentation: [time]
   ```

3. **Required Changes**
   ```
   KEY CHANGES REQUIRED:
   1. [Change 1]
      - Files affected: [number/list]
      - Complexity: [Low/Medium/High]
      - Example: [code example]
   
   2. [Change 2]
      - Files affected: [number/list]
      - Complexity: [Low/Medium/High]
   ```

4. **Testing Requirements**
   ```
   TESTING REQUIREMENTS:
   - Unit tests: [what to test]
   - Integration tests: [what to test]
   - E2E tests: [what to test]
   - Manual testing: [what to verify]
   ```

---

## Complete Package Intelligence Report Format

```
PACKAGE INTELLIGENCE REPORT
===========================

PACKAGE OVERVIEW
---------------
Name: [package-name]
Current Version: [version]
Latest Stable: [version]
Release Date: [date]
Maintainer: [name/org]
License: [license]
GitHub Stars: [number]
Weekly Downloads: [number]

VERSION HISTORY
--------------
- v[latest]: [date] - [major changes]
- v[previous]: [date] - [major changes]
- v[older]: [date] - [major changes]

BREAKING CHANGES
---------------
[If upgrading from v[old] to v[new]]

1. [Breaking Change 1]
   - Impact: [High/Medium/Low]
   - Affects: [what code]
   - Migration:
     ```[language]
     // Before
     [old code]
     
     // After
     [new code]
     ```

2. [Breaking Change 2]
   - Impact: [High/Medium/Low]
   - Affects: [what code]
   - Migration: [steps]

NEW FEATURES
-----------
1. [Feature 1]
   - Description: [what it does]
   - Use case: [when to use]
   - Example:
     ```[language]
     [code example]
     ```

2. [Feature 2]
   - Description: [what it does]
   - Use case: [when to use]

DEPRECATIONS
-----------
1. [Deprecated API 1]
   - Deprecated in: v[version]
   - Will be removed in: v[version]
   - Replacement: [new API]
   - Migration guide: [URL]

SECURITY UPDATES
---------------
[If applicable]
- [CVE-XXXX-XXXX]: [description]
  - Severity: [level]
  - Fixed in: v[version]
  - Action required: [what to do]

COMPATIBILITY
------------
Framework Compatibility:
- [Framework 1]: v[range] ✅
- [Framework 2]: v[range] ⚠️ (notes)
- [Framework 3]: v[range] ❌ (incompatible)

Peer Dependencies:
- [dep-1]: v[range] ✅
- [dep-2]: v[range] ⚠️ (may need update)

Runtime Requirements:
- Node.js: v[range]
- npm/yarn: v[range]
- OS: [requirements]

MIGRATION GUIDANCE
-----------------
Complexity: [Low/Medium/High]
Estimated Effort: [time estimate]

Migration Steps:
1. [Step 1]
2. [Step 2]
3. [Step 3]

Testing Checklist:
- [ ] [Test 1]
- [ ] [Test 2]
- [ ] [Test 3]

Rollback Plan:
If issues occur:
1. [Rollback step 1]
2. [Rollback step 2]

ECOSYSTEM IMPACT
---------------
- Related packages: [list with status]
- Plugins affected: [list]
- Tools affected: [list]

RECOMMENDATION
-------------
[Upgrade/Wait/Alternative] - [Rationale]

Upgrade Priority: [High/Medium/Low]
Risk Level: [Low/Medium/High]

Reasons to upgrade:
- [Reason 1]
- [Reason 2]

Reasons to wait:
- [Reason 1]
- [Reason 2]

SOURCES
-------
- Official docs: [URL]
- Release notes: [URL]
- Migration guide: [URL]
- GitHub releases: [URL]
- npm registry: [URL]

LAST UPDATED
-----------
[Date] - Information verified as of this date
```

---

## Package Comparison Workflow

**When comparing multiple packages:**

### Comparison Matrix

```
PACKAGE COMPARISON
=================

Comparing: [Package A] vs [Package B] vs [Package C]

FEATURE COMPARISON
-----------------
| Feature | Package A | Package B | Package C |
|---------|-----------|-----------|-----------|
| [Feature 1] | ✅ | ✅ | ❌ |
| [Feature 2] | ✅ | ⚠️ Limited | ✅ |
| [Feature 3] | ❌ | ✅ | ✅ |

PERFORMANCE
----------
| Metric | Package A | Package B | Package C |
|--------|-----------|-----------|-----------|
| Bundle size | [size] | [size] | [size] |
| Load time | [time] | [time] | [time] |
| Memory usage | [usage] | [usage] | [usage] |

ECOSYSTEM
---------
| Aspect | Package A | Package B | Package C |
|--------|-----------|-----------|-----------|
| GitHub stars | [number] | [number] | [number] |
| Weekly downloads | [number] | [number] | [number] |
| Last updated | [date] | [date] | [date] |
| Maintainers | [number] | [number] | [number] |
| Open issues | [number] | [number] | [number] |

DEVELOPER EXPERIENCE
-------------------
| Aspect | Package A | Package B | Package C |
|--------|-----------|-----------|-----------|
| Documentation | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ |
| TypeScript support | ✅ Built-in | ✅ Built-in | ⚠️ @types |
| Learning curve | Low | Medium | High |
| Community support | Excellent | Good | Fair |

PROS & CONS
----------
Package A:
Pros:
- [Pro 1]
- [Pro 2]

Cons:
- [Con 1]
- [Con 2]

Package B:
Pros:
- [Pro 1]
- [Pro 2]

Cons:
- [Con 1]
- [Con 2]

USE CASE FIT
-----------
Choose Package A if:
- [Condition 1]
- [Condition 2]

Choose Package B if:
- [Condition 1]
- [Condition 2]

Choose Package C if:
- [Condition 1]
- [Condition 2]

RECOMMENDATION
-------------
For your use case: [Recommendation]
Rationale: [Explanation]

Alternative: [Alternative package]
When to consider: [Conditions]
```

---

## Quality Assurance Checklist

Before providing package intelligence:

- [ ] Latest version verified from official source
- [ ] Release notes reviewed
- [ ] Breaking changes identified
- [ ] Compatibility checked
- [ ] Migration complexity assessed
- [ ] Security updates noted
- [ ] Ecosystem impact evaluated
- [ ] Sources cited with URLs
- [ ] Recommendation provided
- [ ] Risk level assessed

---

## Special Cases

### Case 1: Major Version Upgrade

```
⚠️ MAJOR VERSION UPGRADE

Upgrading from v[old] to v[new] is a MAJOR version change.

EXPECT:
- Breaking changes
- API changes
- Significant migration effort

RECOMMENDATION:
1. Review full changelog
2. Test in development first
3. Allocate time for migration
4. Have rollback plan ready

Migration Guide: [URL]
```

### Case 2: Security Vulnerability

```
🚨 SECURITY VULNERABILITY DETECTED

CVE-[number]: [description]
Severity: [Critical/High/Medium/Low]
Affected versions: [range]
Fixed in: v[version]

ACTION REQUIRED:
1. Upgrade to v[version] immediately
2. Review security advisory: [URL]
3. Check if your code is affected
4. Test thoroughly after upgrade

DO NOT DELAY - Security risk present
```

### Case 3: Deprecated Package

```
⚠️ PACKAGE DEPRECATED

This package is no longer maintained.

Last update: [date]
Deprecation notice: [URL]

RECOMMENDED ALTERNATIVES:
1. [Alternative 1] - [why]
2. [Alternative 2] - [why]

Migration path: [guidance]
```

---

This workflow ensures comprehensive package intelligence with verified information and clear migration guidance.
