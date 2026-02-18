---
name: "kiro-web-intelligence-suite"
displayName: "Kiro Web Intelligence Suite"
description: "Production-grade web research, documentation intelligence, error analysis, package verification, and ecosystem monitoring system with multi-source verification"
version: "2.0.0"
author: "NitionzPvtLtd Development Team"
category: "Knowledge & Research"
keywords: ["web search", "documentation", "error debugging", "stackoverflow", "github", "npm", "packages", "migration guide", "version check", "compatibility", "best practices", "release notes", "api reference", "framework updates", "ecosystem intelligence", "production research"]
---

# 🚀 Kiro Web Intelligence Suite

## Mission Statement

Provide **structured, verified, multi-source web research** with production-grade synthesis for professional development workflows. This is not just web search - it's an intelligent research system designed for agencies, SaaS founders, freelancers, and enterprise teams.

## Core Value Proposition

- ⚡ **Faster Debugging** - Structured error intelligence with verified solutions
- 🎯 **Accurate Migration Planning** - Multi-source verification of breaking changes
- � **Verified Ecosystem Intelligence** - Cross-referenced package information
- 🛡️ **Reduced Production Risk** - Source validation and compatibility checks
- 📊 **Professional-Grade Research** - Structured output with traceability

---

## When to Load Steering Files

This power includes specialized steering files for different research workflows. Kiro will automatically load the appropriate file based on your task:

- **Error debugging and troubleshooting** → `error-intelligence-workflow.md`
- **Package research and version checking** → `package-intelligence-workflow.md`
- **Migration planning and breaking changes** → `migration-planning-workflow.md`
- **Code pattern research and examples** → `code-pattern-research-workflow.md`
- **Multi-source verification for critical decisions** → `verification-protocol-workflow.md`

When you're debugging an error, Kiro loads `error-intelligence-workflow.md`. When you switch to checking package versions, it loads `package-intelligence-workflow.md` instead. This prevents overwhelming context with every pattern upfront.

---

## Operational Capabilities Matrix

## Operational Capabilities Matrix

### 🎯 Capability 1: Structured Web Research Protocol

**Tool:** `remote_web_search`

**Primary Functions:**
- Retrieve current documentation with version context
- Identify breaking changes across releases
- Research migration paths with risk assessment
- Compare frameworks/libraries with tradeoff analysis
- Verify ecosystem updates and compatibility

**Operational Rules:**
1. **Source Priority Hierarchy:**
   - 1️⃣ Official Documentation (highest trust)
   - 2️⃣ Official GitHub Repository
   - 3️⃣ Maintainer Blog Posts
   - 4️⃣ High-quality Community Sources
   - 5️⃣ Stack Overflow (verified answers only)

2. **Quality Filters:**
   - Prefer sources with publication dates
   - Avoid outdated sources (>2 years for fast-moving tech)
   - Include version numbers when applicable
   - Cross-check with minimum 2 sources for critical decisions

3. **Search Strategy:**
   - Start broad, narrow down
   - Include version numbers in queries
   - Use exact error strings
   - Specify framework/library context

**Example Queries:**
```
"Next.js 15 App Router breaking changes"
"React 19 migration guide official"
"TypeScript 5.x strict mode compatibility"
"Firebase v10 authentication changes"
```

---

### 📄 Capability 2: Authoritative Documentation Fetching

**Tool:** `webFetch`

**Primary Functions:**
- Retrieve official documentation pages
- Extract API references with parameter details
- Analyze release notes for breaking changes
- Parse migration guides with step-by-step instructions

**Fetch Modes:**
- **Truncated** (8KB): Quick preview, initial assessment
- **Full** (10MB): Deep analysis, comprehensive extraction
- **Selective**: Target specific APIs or sections

**Operational Protocol:**
1. **Pre-Fetch Validation:**
   - Verify URL is from official source
   - Check if documentation is current version
   - Confirm URL accessibility

2. **Post-Fetch Processing:**
   - Extract key information
   - Identify version-specific details
   - Note deprecation warnings
   - Highlight breaking changes

3. **Content Synthesis:**
   - Summarize key points
   - Extract code examples
   - Identify best practices
   - Note compatibility requirements

**Best Practices:**
- Use full mode for migration guides
- Use selective mode for specific API lookups
- Always verify version matches user's context

---

### 🐛 Capability 3: Error Intelligence System

**Activation:** When user provides error message or error code

**Multi-Phase Protocol:**

**Phase 1: Error Classification**
- Identify error type (syntax, runtime, configuration, network)
- Determine severity (critical, high, medium, low)
- Extract error code and message
- Identify affected framework/library

**Phase 2: Structured Search**
1. Search exact error string with quotes
2. Include framework and version context
3. Prioritize sources:
   - Official documentation error pages
   - GitHub issues (open and closed)
   - Stack Overflow accepted answers
   - Framework-specific forums

**Phase 3: Solution Extraction**
Extract and structure:
- **Root Cause:** Why error occurs
- **Common Triggers:** What causes it
- **Verified Solutions:** Step-by-step fixes
- **Prevention Strategies:** How to avoid
- **Version Context:** Which versions affected
- **Compatibility Notes:** Framework interactions

**Phase 4: Solution Validation**
- Verify solution is for correct version
- Check if solution is still valid
- Identify any side effects
- Confirm compatibility with user's stack

**Output Format:**
```
ERROR INTELLIGENCE REPORT
========================

Error: [error code/message]
Framework: [name] v[version]
Severity: [level]

ROOT CAUSE:
[Explanation]

COMMON TRIGGERS:
1. [Trigger 1]
2. [Trigger 2]

VERIFIED SOLUTIONS:
Solution 1: [Step-by-step]
- Source: [URL]
- Verified: [date/version]
- Success Rate: [if available]

Solution 2: [Alternative]
- Source: [URL]
- Verified: [date/version]

PREVENTION:
- [Strategy 1]
- [Strategy 2]

COMPATIBILITY NOTES:
- [Important compatibility info]

SOURCES:
- [URL 1]
- [URL 2]
```

---

### 📦 Capability 4: Package & Version Intelligence

**Activation:** Version checks, package research, compatibility verification

**Intelligence Gathering Protocol:**

**Phase 1: Version Discovery**
- Check official package registry (npm, PyPI, etc.)
- Verify latest stable version
- Identify beta/canary versions
- Check release frequency

**Phase 2: Release Analysis**
- Fetch release notes
- Identify breaking changes
- Extract new features
- Note deprecations
- Check security updates

**Phase 3: Compatibility Matrix**
- Verify peer dependencies
- Check framework compatibility
- Identify version conflicts
- Assess ecosystem impact

**Phase 4: Migration Assessment**
- Identify migration path
- Estimate migration complexity
- List required code changes
- Note testing requirements

**Output Format:**
```
PACKAGE INTELLIGENCE REPORT
===========================

Package: [name]
Current Version: [version]
Latest Stable: [version]
Release Date: [date]

BREAKING CHANGES:
- [Change 1] (affects: [area])
- [Change 2] (affects: [area])

NEW FEATURES:
- [Feature 1]
- [Feature 2]

DEPRECATIONS:
- [Deprecated API 1] → [Replacement]
- [Deprecated API 2] → [Replacement]

COMPATIBILITY:
- Framework: [name] v[version] ✅/⚠️/❌
- Dependencies: [status]
- Node.js: [version range]

MIGRATION GUIDANCE:
Complexity: [Low/Medium/High]
Estimated Effort: [hours/days]
Key Changes Required:
1. [Change 1]
2. [Change 2]

ECOSYSTEM IMPACT:
- [Impact on related packages]

SOURCES:
- [Official release notes URL]
- [Migration guide URL]
```

---

### 💻 Capability 5: Code Pattern Intelligence

**Activation:** Code examples, pattern research, implementation guidance

**Pattern Extraction Protocol:**

**Phase 1: Pattern Discovery**
- Search authoritative examples
- Identify official patterns
- Find community best practices
- Locate real-world implementations

**Phase 2: Pattern Analysis**
- Extract clean patterns
- Understand architecture decisions
- Identify tradeoffs
- Note performance implications

**Phase 3: Context Adaptation**
- Adapt for user's framework version
- Adjust for user's use case
- Modernize if pattern is outdated
- Add type safety if applicable

**Phase 4: Implementation Guidance**
- Provide step-by-step implementation
- Include error handling
- Add testing recommendations
- Note edge cases

**Quality Standards:**
- Never copy blindly without understanding
- Always verify compatibility with user's version
- Explain why pattern works
- Provide alternatives when applicable

**Output Format:**
```
CODE PATTERN INTELLIGENCE
=========================

Pattern: [name]
Use Case: [description]
Framework: [name] v[version]

PATTERN OVERVIEW:
[High-level explanation]

ARCHITECTURE DECISIONS:
- [Decision 1]: [Rationale]
- [Decision 2]: [Rationale]

IMPLEMENTATION:
```[language]
[Clean, adapted code]
```

TRADEOFFS:
Pros:
- [Pro 1]
- [Pro 2]

Cons:
- [Con 1]
- [Con 2]

ALTERNATIVES:
- [Alternative 1]: [When to use]
- [Alternative 2]: [When to use]

TESTING STRATEGY:
- [Test approach]

EDGE CASES:
- [Edge case 1]: [How to handle]

SOURCES:
- [Official docs URL]
- [Example implementation URL]
```

---

### 🔍 Capability 6: Multi-Source Verification Mode

**Activation:** Critical decisions, production deployments, major migrations

**Verification Protocol:**

**Phase 1: Source Collection**
- Gather minimum 3 sources
- Include official documentation
- Add community verification
- Check recent discussions

**Phase 2: Cross-Reference Analysis**
- Compare information across sources
- Identify consensus
- Flag conflicting information
- Assess source credibility

**Phase 3: Conflict Resolution**
- Prioritize official sources
- Check publication dates
- Verify with latest version
- Test if possible

**Phase 4: Risk Assessment**
- Identify potential risks
- Assess impact of conflicts
- Recommend safest option
- Provide fallback strategies

**Output Format:**
```
MULTI-SOURCE VERIFICATION REPORT
================================

Query: [research question]
Sources Analyzed: [number]
Consensus Level: [High/Medium/Low]

SOURCE 1: [Official Docs]
- Information: [summary]
- Date: [date]
- Credibility: ⭐⭐⭐⭐⭐

SOURCE 2: [GitHub Issue]
- Information: [summary]
- Date: [date]
- Credibility: ⭐⭐⭐⭐

SOURCE 3: [Stack Overflow]
- Information: [summary]
- Date: [date]
- Credibility: ⭐⭐⭐

CONSENSUS:
[What all sources agree on]

CONFLICTS:
- Conflict 1: [Description]
  - Source A says: [info]
  - Source B says: [info]
  - Resolution: [recommended approach]

RISK ASSESSMENT:
- Risk Level: [Low/Medium/High]
- Key Risks: [list]
- Mitigation: [strategies]

RECOMMENDATION:
[Safest, most verified approach]

FALLBACK STRATEGY:
[Alternative if primary fails]
```

---

## Decision-Making Framework

### Source Trust Hierarchy

**Tier 1: Absolute Trust**
- Official documentation (current version)
- Official GitHub repository
- Official blog posts from maintainers

**Tier 2: High Trust**
- Verified Stack Overflow answers (accepted, high votes)
- Well-maintained community docs
- Recent GitHub issues with maintainer responses

**Tier 3: Moderate Trust**
- Popular blog posts (with verification)
- Conference talks from maintainers
- Community tutorials (recent, verified)

**Tier 4: Low Trust**
- Unverified blog posts
- Old tutorials (>2 years)
- Forum posts without verification

**Tier 5: No Trust**
- AI-generated content without sources
- Outdated documentation
- Unverified claims

### Version Context Rules

**Always Include:**
- Framework version
- Language version
- Major dependency versions
- Platform/environment

**When Version Not Specified:**
1. Ask user for version if critical
2. Default to latest stable version
3. Explicitly state assumption
4. Provide version-specific guidance

**Version Compatibility Checks:**
- Verify compatibility before suggesting
- Note breaking changes between versions
- Provide migration path if needed
- Warn about deprecated features

---

## Failure Handling Protocol

### Scenario 1: No Reliable Source Found

**Response:**
```
⚠️ RESEARCH LIMITATION DETECTED

I searched for: [query]
Sources checked: [number]
Reliable sources found: 0

ISSUE:
- No official documentation found
- Community sources are outdated/conflicting
- Version-specific information unavailable

RECOMMENDATION:
1. Refine search with more specific terms
2. Specify exact version numbers
3. Check if feature/API exists in your version
4. Consider alternative approaches

Would you like me to:
- Search with different terms?
- Check alternative sources?
- Research related topics?
```

### Scenario 2: Version Mismatch Detected

**Response:**
```
⚠️ VERSION MISMATCH WARNING

Your version: [version]
Documentation found: [version]
Compatibility: ⚠️ Uncertain

RISKS:
- API may have changed
- Breaking changes possible
- Behavior may differ

RECOMMENDATION:
1. Verify your exact version
2. Check changelog between versions
3. Test in development first
4. Consider upgrading if feasible

Proceed with caution.
```

### Scenario 3: Conflicting Information

**Response:**
```
⚠️ CONFLICTING INFORMATION DETECTED

Source 1 says: [info]
Source 2 says: [different info]

ANALYSIS:
- Source 1: [credibility assessment]
- Source 2: [credibility assessment]

RECOMMENDATION:
Based on source credibility and recency, I recommend: [approach]

VERIFICATION NEEDED:
- Test in your environment
- Check official docs
- Verify with your version

Risk Level: [assessment]
```

---

## Professional Mode Activation

### When to Activate

- Production deployments
- Major migrations
- Critical bug fixes
- Architecture decisions
- Security-related research

### Professional Mode Behavior

**Tone:** Formal, technical, precise

**Output Structure:**
1. Executive Summary
2. Detailed Analysis
3. Risk Assessment
4. Recommendations
5. Implementation Plan
6. Verification Steps

**Additional Requirements:**
- Include tradeoff analysis
- Provide risk mitigation strategies
- Offer multiple approaches
- Include rollback plans
- Add monitoring recommendations

**Example Output:**
```
PROFESSIONAL RESEARCH REPORT
============================

EXECUTIVE SUMMARY
-----------------
[High-level overview]

DETAILED ANALYSIS
-----------------
[Comprehensive breakdown]

RISK ASSESSMENT
---------------
Risk Level: [High/Medium/Low]
Key Risks:
1. [Risk 1] - Impact: [level]
2. [Risk 2] - Impact: [level]

Mitigation Strategies:
1. [Strategy 1]
2. [Strategy 2]

RECOMMENDATIONS
---------------
Primary: [Recommendation]
Rationale: [Why]

Alternative: [Alternative]
When to use: [Conditions]

IMPLEMENTATION PLAN
-------------------
Phase 1: [Steps]
Phase 2: [Steps]
Phase 3: [Steps]

VERIFICATION STEPS
------------------
1. [Verification 1]
2. [Verification 2]

ROLLBACK PLAN
-------------
If issues occur:
1. [Rollback step 1]
2. [Rollback step 2]

MONITORING
----------
Monitor these metrics:
- [Metric 1]
- [Metric 2]
```

---

## Activation Logic & Triggers

### High-Confidence Activation

**Exact Triggers:**
- "search for [topic]"
- "look up [error]"
- "latest version of [package]"
- "documentation for [framework]"
- "fetch docs from [URL]"
- "error: [error message]"
- "stack overflow [topic]"
- "github issue [topic]"
- "migration guide [framework]"
- "compare [package A] vs [package B]"
- "best practices [topic]"
- "breaking changes [package]"

**Pattern Triggers:**
- Questions about versions
- Error messages in quotes
- Requests for documentation
- Package comparison requests
- Migration planning queries
- Compatibility questions

### Context-Based Activation

**Activate when user mentions:**
- Specific error codes
- Package names with versions
- Framework updates
- API changes
- Deprecation warnings
- Security vulnerabilities

---

## Output Standards & Quality Control

### Every Research Response Must Include

**1. Source Validation Summary**
```
SOURCES VERIFIED:
✅ Official Documentation - [URL]
✅ GitHub Repository - [URL]
⚠️ Community Source - [URL] (verify independently)
```

**2. Version Context**
```
VERSION CONTEXT:
- Framework: [name] v[version]
- Language: [name] v[version]
- Platform: [details]
- Last Updated: [date]
```

**3. Risk Warnings (if applicable)**
```
⚠️ RISK WARNINGS:
- Breaking changes in v[version]
- Deprecated API usage
- Compatibility concerns with [dependency]
```

**4. Implementation Guidance**
```
IMPLEMENTATION:
1. [Step 1]
2. [Step 2]
3. [Step 3]

TESTING:
- [Test approach]

VERIFICATION:
- [How to verify it works]
```

**5. Verification Recommendation**
```
VERIFICATION RECOMMENDED:
- Test in development environment
- Check with your specific version
- Verify dependencies are compatible
- Review official changelog
```

---

## Limitations & Constraints

### Cannot Access

❌ **Authenticated Content**
- Private repositories
- Paywalled content
- Login-required documentation
- Internal company docs

❌ **Dynamic Content**
- JavaScript-rendered pages (limited)
- Interactive web applications
- Real-time data feeds
- Database queries

❌ **Executable Operations**
- Cannot run code
- Cannot test solutions
- Cannot deploy changes
- Cannot access production systems

### Can Access

✅ **Public Content**
- Official documentation
- Public GitHub repositories
- Stack Overflow
- Public blogs and articles
- npm/PyPI package registries
- Release notes and changelogs

---

## Advanced Research Workflows

### Workflow 1: Complete Error Resolution

```
USER: "Error: auth/invalid-credential in Firebase"

KIRO EXECUTES:
1. Search exact error with Firebase context
2. Fetch official Firebase error documentation
3. Search Stack Overflow for solutions
4. Check GitHub issues
5. Synthesize multi-source solution
6. Provide structured error intelligence report

OUTPUT: Complete error intelligence with verified solutions
```

### Workflow 2: Migration Planning

```
USER: "Plan migration from Next.js 14 to 15"

KIRO EXECUTES:
1. Fetch Next.js 15 release notes
2. Identify breaking changes
3. Search for migration guides
4. Check community experiences
5. Assess compatibility with dependencies
6. Create structured migration plan

OUTPUT: Professional migration report with risk assessment
```

### Workflow 3: Package Comparison

```
USER: "Compare Zustand vs Redux Toolkit"

KIRO EXECUTES:
1. Fetch documentation for both
2. Compare features and APIs
3. Research performance benchmarks
4. Check community adoption
5. Analyze use case fit
6. Provide tradeoff analysis

OUTPUT: Comprehensive comparison with recommendations
```

### Workflow 4: Version Verification

```
USER: "What's the latest React version and what's new?"

KIRO EXECUTES:
1. Check npm registry for latest version
2. Fetch release notes
3. Identify new features
4. Check breaking changes
5. Assess migration complexity
6. Provide version intelligence report

OUTPUT: Complete version intelligence with upgrade guidance
```

---

## Training Data Integration

### Leveraging Training Knowledge (up to April 2024)

**Strengths:**
- Solid foundation in fundamentals
- Understanding of core concepts
- Knowledge of established patterns
- Historical context

**Combined with Web Search:**
- Current version information
- Latest features and APIs
- Recent breaking changes
- Up-to-date best practices

**Best of Both Worlds:**
```
Training Knowledge: React fundamentals, hooks patterns
+ Web Search: React 19 new features, Server Components
= Complete, current understanding
```

---

## Professional Use Cases

### For Agencies

**Value:**
- Faster client project research
- Verified technology recommendations
- Risk-assessed migration planning
- Professional documentation

**Example:**
"Research authentication solutions for e-commerce client - need production-grade comparison"

### For SaaS Founders

**Value:**
- Quick technology validation
- Ecosystem compatibility checks
- Breaking change monitoring
- Competitive analysis

**Example:**
"Verify if Stripe API v2024 is compatible with our Next.js 15 stack"

### For Freelancers

**Value:**
- Rapid problem solving
- Client-ready documentation
- Technology learning
- Best practice verification

**Example:**
"Client needs Firebase migration from v9 to v10 - provide migration plan"

### For Enterprise Teams

**Value:**
- Multi-source verification
- Risk assessment
- Compliance checking
- Audit trail documentation

**Example:**
"Assess security implications of upgrading to Node.js 20 LTS"

---

## Quality Assurance Checklist

Before providing any research output, verify:

- [ ] Sources are from trusted tier (1-3)
- [ ] Version context is clear
- [ ] Information is current (check dates)
- [ ] Multiple sources confirm (for critical info)
- [ ] Risks are identified and communicated
- [ ] Implementation guidance is provided
- [ ] Verification steps are included
- [ ] Limitations are disclosed
- [ ] Sources are cited with URLs

---

## Never Fabricate Rule

**Absolute Rule:** If information cannot be found or verified:

1. ✅ Explicitly state limitation
2. ✅ Explain what was searched
3. ✅ Suggest alternative approaches
4. ✅ Offer to refine search

❌ **NEVER:**
- Make up information
- Guess at solutions
- Provide unverified claims
- Assume without stating

**Example Response:**
```
I searched for [query] across official docs, GitHub, and Stack Overflow, 
but couldn't find reliable information for your specific version.

This could mean:
- Feature doesn't exist in your version
- Documentation is incomplete
- Very new/experimental feature

Would you like me to:
1. Search for alternative approaches?
2. Check if feature exists in newer versions?
3. Research related solutions?
```

---

## Continuous Improvement

### Feedback Integration

When user reports:
- Outdated information → Note source date
- Incorrect solution → Verify and update approach
- Missing context → Add to future queries

### Learning from Usage

Track patterns:
- Common error types
- Frequently researched topics
- Successful solution patterns
- Source reliability

---

## Version History

**v2.0.0** - Production Release
- Structured intelligence protocols
- Multi-source verification
- Professional mode
- Risk assessment framework
- Quality assurance standards

**v1.0.0** - Initial Release
- Basic web search
- Documentation fetching
- Error lookup

---

## Conclusion

The Kiro Web Intelligence Suite is not just a search tool - it's a **production-grade research system** designed for professional developers who need:

- ✅ Verified information
- ✅ Structured output
- ✅ Risk assessment
- ✅ Multi-source validation
- ✅ Professional documentation

**Use this power when you need research you can trust for production systems.**

### ✅ Web Search

**Capability:** Search the entire web using `remote_web_search` tool

**What You Can Search For:**
- Current documentation and tutorials
- Error messages and solutions
- Package information and versions
- Code examples and patterns
- Best practices and guides
- API references
- Framework updates
- Library comparisons

**How to Use:**
```
"Search for Next.js 15 App Router documentation"
"Look up Firebase authentication error solutions"
"Find React 19 hooks best practices"
"Search for TypeScript strict mode migration guide"
```

**What Happens:**
1. Kiro searches the web
2. Returns relevant results with URLs
3. Can fetch and read the content
4. Provides synthesized answer with sources

---

### ✅ Fetch Documentation

**Capability:** Fetch and read content from specific URLs using `webFetch` tool

**What You Can Fetch:**
- Official documentation pages
- GitHub README files
- Blog posts and tutorials
- API references
- Stack Overflow answers
- Package documentation
- Release notes
- Migration guides

**How to Use:**
```
"Fetch and read https://nextjs.org/docs/app/building-your-application/routing"
"Read the Firebase Auth documentation from [URL]"
"Get the latest from React's official blog"
```

**Modes Available:**
- **Truncated** (default): First 8KB for quick preview
- **Full**: Complete content up to 10MB
- **Selective**: Only sections containing specific phrase

---

### ✅ Look Up Errors

**Capability:** Search for error messages and find solutions

**What You Can Do:**
- Search for exact error messages
- Find Stack Overflow solutions
- Read GitHub issues
- Check documentation for errors
- Learn from others' solutions

**How to Use:**
```
"Search for 'Firebase auth/invalid-credential error'"
"Look up 'Next.js hydration mismatch' solutions"
"Find solutions for 'TypeScript TS2345 error'"
"Search Stack Overflow for React useEffect cleanup"
```

**Best Practice:**
- Provide the exact error message
- Include relevant context (framework, version)
- Kiro will find and synthesize solutions

---

### ✅ Check Package Versions

**Capability:** Look up latest package versions and documentation

**What You Can Check:**
- Latest npm package versions
- Package documentation
- Breaking changes
- Migration guides
- Compatibility information
- Deprecation notices

**How to Use:**
```
"What's the latest version of Next.js?"
"Check if React 19 has breaking changes"
"Look up Firebase SDK latest version"
"Find TypeScript 5.x migration guide"
```

**What You Get:**
- Current version numbers
- Release notes
- Breaking changes
- Migration instructions
- Compatibility info

---

### ✅ Read Code Examples

**Capability:** Fetch and learn from code examples online

**Where Kiro Can Read From:**
- GitHub repositories (public)
- Stack Overflow code snippets
- Documentation code examples
- Blog post code samples
- Tutorial code
- Open source projects

**How to Use:**
```
"Show me React Server Components examples from Next.js docs"
"Find Firebase authentication code examples"
"Look up TypeScript generic patterns on GitHub"
"Get code examples for Zustand state management"
```

**What Kiro Does:**
1. Searches for relevant code
2. Fetches the code examples
3. Reads and understands the code
4. Explains how it works
5. Adapts it to your needs

---

### ✅ Learn Current Best Practices

**Capability:** Research and learn from current online resources

**What Kiro Can Learn:**
- Latest framework patterns
- Current best practices
- New API features
- Modern coding techniques
- Performance optimizations
- Security recommendations

**How to Use:**
```
"What are the current React 19 best practices?"
"Learn about Next.js 15 caching strategies"
"Find modern TypeScript patterns"
"Research Firebase security rules best practices"
```

**Advantage:**
- Combines training knowledge (up to April 2024)
- With current web information
- Best of both worlds

---

## How It Works

### Web Search Flow

1. **You Ask:** "Search for Next.js 15 App Router guide"
2. **Kiro Searches:** Uses `remote_web_search` tool
3. **Results Returned:** List of relevant URLs with snippets
4. **Kiro Reads:** Fetches most relevant pages
5. **Answer Provided:** Synthesized information with sources

### Fetch Flow

1. **You Provide URL:** "Read https://nextjs.org/docs/..."
2. **Kiro Fetches:** Uses `webFetch` tool
3. **Content Retrieved:** Full page content
4. **Kiro Understands:** Reads and comprehends
5. **Answer Provided:** Relevant information extracted

---

## Best Practices

### 🎯 Be Specific

**Good:**
```
"Search for Next.js 15 App Router data fetching patterns"
"Look up Firebase v10 authentication migration guide"
"Find React 19 useTransition hook examples"
```

**Less Effective:**
```
"Search for Next.js stuff"
"Look up Firebase"
"Find React examples"
```

**Why:** Specific queries return more relevant results

---

### 🔗 Provide URLs When Known

**Good:**
```
"Fetch and read https://nextjs.org/docs/app/api-reference/functions/fetch"
"Read the Firebase Auth docs at [specific URL]"
```

**Also Good:**
```
"Search for Next.js fetch documentation"
```

**Why:** Direct URLs are faster, but search works great too

---

### 📝 Include Context

**Good:**
```
"Search for 'hydration mismatch' error in Next.js 15"
"Look up TypeScript 5.3 strict mode issues"
"Find React 19 Server Components examples"
```

**Less Effective:**
```
"Search for hydration error"
"Look up TypeScript issues"
"Find React examples"
```

**Why:** Context helps find relevant solutions

---

### 🔄 Verify Across Sources

**Good Practice:**
```
"Search for Next.js caching strategies and verify across multiple sources"
"Look up Firebase security rules best practices from official docs and community"
```

**Why:** Multiple sources provide better confidence

---

### 📚 Ask for Learning

**Good:**
```
"Search for and teach me about React Server Components"
"Look up Next.js 15 new features and explain them"
"Find and explain TypeScript 5.x decorators"
```

**Why:** Kiro can research, learn, and teach you

---

## Common Use Cases

### 1. Error Debugging

**Scenario:** You encounter an error

**What to Do:**
```
"Search for 'Firebase Error: auth/invalid-credential' solutions"
"Look up 'Next.js Error: Hydration failed' on Stack Overflow"
"Find GitHub issues for 'TypeScript TS2345 error'"
```

**What Kiro Does:**
1. Searches for the error
2. Finds Stack Overflow answers
3. Reads GitHub issues
4. Checks documentation
5. Provides solution with sources

---

### 2. Learning New Features

**Scenario:** You want to learn a new feature

**What to Do:**
```
"Search for React 19 Server Actions tutorial"
"Look up Next.js 15 Partial Prerendering guide"
"Find TypeScript 5.x satisfies operator examples"
```

**What Kiro Does:**
1. Searches for tutorials
2. Fetches documentation
3. Reads code examples
4. Explains the feature
5. Provides working examples

---

### 3. Checking Compatibility

**Scenario:** You need to check if packages work together

**What to Do:**
```
"Search for Next.js 15 and React 19 compatibility"
"Look up Firebase v10 with TypeScript 5.x compatibility"
"Check if Tailwind CSS 4 works with Next.js 15"
```

**What Kiro Does:**
1. Searches for compatibility info
2. Checks release notes
3. Reads migration guides
4. Verifies versions
5. Provides compatibility report

---

### 4. Finding Best Practices

**Scenario:** You want to follow current best practices

**What to Do:**
```
"Search for Next.js 15 App Router best practices"
"Look up React 19 performance optimization techniques"
"Find TypeScript strict mode migration best practices"
```

**What Kiro Does:**
1. Searches for best practices
2. Reads official guides
3. Checks community recommendations
4. Synthesizes information
5. Provides actionable advice

---

### 5. Package Research

**Scenario:** You're choosing between packages

**What to Do:**
```
"Compare Zustand vs Redux Toolkit for React state management"
"Search for best Next.js form libraries in 2024"
"Look up Firebase alternatives for authentication"
```

**What Kiro Does:**
1. Searches for comparisons
2. Reads documentation
3. Checks GitHub stars/activity
4. Reviews community feedback
5. Provides comparison with pros/cons

---

### 6. Migration Guides

**Scenario:** You need to migrate to a new version

**What to Do:**
```
"Search for Next.js 14 to 15 migration guide"
"Look up React 18 to 19 breaking changes"
"Find Firebase v9 to v10 migration steps"
```

**What Kiro Does:**
1. Finds official migration guides
2. Reads breaking changes
3. Checks community experiences
4. Provides step-by-step guide
5. Highlights important changes

---

## Limitations

### ⚠️ What Kiro CANNOT Do

**Cannot Execute JavaScript:**
- Cannot run JavaScript on pages
- Cannot interact with dynamic content
- Cannot fill forms or click buttons
- Cannot see JavaScript-rendered content

**Cannot Access Authenticated Sites:**
- Cannot log into websites
- Cannot access private repositories
- Cannot read behind paywalls
- Cannot access internal documentation

**Cannot Browse Interactively:**
- Cannot click through multiple pages
- Cannot navigate like a human
- Cannot explore sites dynamically
- Must fetch specific URLs

**Cannot Access Private Resources:**
- Cannot read private GitHub repos
- Cannot access company internal docs
- Cannot read private Stack Overflow teams
- Cannot access restricted content

---

## Training Data Context

### April 2024 Cutoff

**What This Means:**
- Kiro has foundational knowledge up to April 2024
- Can supplement with current web searches
- Best of both: training knowledge + current info

**Example:**
```
Training Knowledge: React 18 patterns (solid foundation)
+ Web Search: React 19 new features (current info)
= Complete understanding of React ecosystem
```

**Best Practice:**
- For fundamentals: Kiro knows from training
- For latest features: Kiro searches the web
- For current versions: Kiro checks online
- For recent changes: Kiro fetches docs

---

## Advanced Techniques

### 1. Multi-Source Verification

**Technique:** Verify information across multiple sources

**How to Use:**
```
"Search for Next.js caching strategies from:
1. Official Next.js documentation
2. Vercel blog posts
3. Community best practices
Then synthesize the information"
```

**Benefit:** Higher confidence in accuracy

---

### 2. Comparative Research

**Technique:** Compare multiple approaches or tools

**How to Use:**
```
"Search for and compare:
1. Next.js App Router vs Pages Router
2. Read pros and cons from multiple sources
3. Provide recommendation for my use case"
```

**Benefit:** Informed decision making

---

### 3. Deep Dive Learning

**Technique:** Research a topic thoroughly

**How to Use:**
```
"Research React Server Components:
1. Search for official documentation
2. Find tutorial articles
3. Look up code examples
4. Check common pitfalls
5. Provide comprehensive guide"
```

**Benefit:** Complete understanding

---

### 4. Error Pattern Analysis

**Technique:** Research error patterns and solutions

**How to Use:**
```
"Search for 'hydration mismatch' errors:
1. Find common causes
2. Look up solutions on Stack Overflow
3. Check Next.js documentation
4. Provide prevention strategies"
```

**Benefit:** Prevent future errors

---

### 5. Version-Specific Research

**Technique:** Research specific version features

**How to Use:**
```
"Search for Next.js 15.5.7 specific features:
1. Check release notes
2. Find breaking changes
3. Look up new APIs
4. Provide migration guide"
```

**Benefit:** Version-accurate information

---

## Examples

### Example 1: Debugging an Error

**You:**
```
I'm getting this error: "Firebase Error: auth/invalid-credential"
Search for solutions and explain what it means.
```

**Kiro Will:**
1. Search for the error message
2. Find Stack Overflow answers
3. Read Firebase documentation
4. Check GitHub issues
5. Provide explanation and solutions

**Result:**
- Error explanation
- Common causes
- Step-by-step solutions
- Prevention tips
- Links to sources

---

### Example 2: Learning New Feature

**You:**
```
Search for React 19 Server Actions and teach me how to use them
with Next.js 15 App Router.
```

**Kiro Will:**
1. Search for Server Actions docs
2. Fetch Next.js documentation
3. Find code examples
4. Read tutorials
5. Provide comprehensive guide

**Result:**
- Feature explanation
- Working code examples
- Best practices
- Common pitfalls
- Integration guide

---

### Example 3: Package Research

**You:**
```
I need a form library for Next.js 15. Search for the best options
and compare them.
```

**Kiro Will:**
1. Search for Next.js form libraries
2. Check npm packages
3. Read documentation
4. Compare features
5. Provide recommendations

**Result:**
- List of options
- Feature comparison
- Pros and cons
- Recommendation
- Getting started guide

---

### Example 4: Version Check

**You:**
```
What's the latest version of Next.js and what are the new features?
```

**Kiro Will:**
1. Search for Next.js releases
2. Check npm registry
3. Read release notes
4. Find feature announcements
5. Provide summary

**Result:**
- Current version
- New features
- Breaking changes
- Migration guide
- Links to docs

---

## Tips for Success

### ✅ DO

- Be specific in your searches
- Provide error messages exactly
- Include version numbers
- Ask for multiple sources
- Request code examples
- Ask Kiro to explain findings
- Verify critical information

### ❌ DON'T

- Be too vague
- Assume Kiro knows your exact setup
- Skip version information
- Trust blindly without testing
- Forget to test suggestions
- Ignore source links

---

## Troubleshooting

### Search Returns No Results

**Possible Causes:**
- Query too specific
- Typo in search terms
- Very new/obscure topic

**Solutions:**
- Broaden search terms
- Check spelling
- Try alternative keywords
- Search for related topics

---

### Fetched Content Not Helpful

**Possible Causes:**
- Wrong URL
- Page structure changed
- Content behind JavaScript

**Solutions:**
- Try different URL
- Search for alternative sources
- Ask Kiro to search instead

---

### Information Seems Outdated

**Possible Causes:**
- Old documentation found
- Cached results
- Deprecated information

**Solutions:**
- Specify "latest" or "current"
- Include version numbers
- Ask for recent sources
- Verify with official docs

---

## Real-World Workflow

### Typical Development Flow

1. **Encounter Issue**
   ```
   "Search for [error message] solutions"
   ```

2. **Research Solution**
   ```
   "Fetch documentation from [URL]"
   ```

3. **Learn Implementation**
   ```
   "Find code examples for [feature]"
   ```

4. **Verify Best Practices**
   ```
   "Search for [feature] best practices"
   ```

5. **Check Compatibility**
   ```
   "Verify [package A] works with [package B]"
   ```

6. **Implement Solution**
   - Test the code
   - Verify it works
   - Document learnings

---

## Conclusion

Kiro's internet access is a powerful capability that combines:
- **Training Knowledge:** Solid foundation up to April 2024
- **Web Search:** Current information from the entire web
- **Documentation Fetching:** Direct access to official docs
- **Code Learning:** Read and understand online examples

**Use it for:**
- 🔍 Researching errors and solutions
- 📚 Learning new features and patterns
- 📦 Checking packages and versions
- 💻 Finding code examples
- 🎓 Staying current with best practices

**Remember:**
- Be specific in your requests
- Provide context and versions
- Verify critical information
- Test all suggestions
- Leverage both training knowledge and web search

**Kiro can research, learn, and help you stay current with the rapidly evolving web development ecosystem!**

---

**This power teaches you how to effectively leverage Kiro's full internet access capabilities for maximum productivity.**
