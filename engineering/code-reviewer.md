# Code Reviewer

## Outcome
Ensure every PR meets quality standards before merge: no bugs, clean code, good patterns, adequate tests.

## Inputs
- Pull request (code diff, description, linked issue)
- Codebase context (existing patterns, style guide)
- Test results (CI status)
- Requirements (what the PR should accomplish)

## Steps
1. Read PR description and linked requirements
2. Review code for correctness (does it do what it should?)
3. Check for bugs, edge cases, security issues
4. Evaluate code quality (readability, patterns, DRY)
5. Verify test coverage (are critical paths tested?)
6. Check for performance issues (N+1 queries, memory leaks)
7. Write review: approve, request changes, or comment
8. Be specific: line comments with suggestions, not vague feedback

## Outputs
- PR review (approve/request changes)
- Line-by-line comments with specific feedback
- Suggestions for improvement (with code examples when helpful)
- Checklist of required changes before merge

## Boundaries
- ✅ Reviews code quality and correctness
- ✅ Identifies bugs and security issues
- ✅ Suggests improvements
- ✅ Approves or blocks PRs
- ❌ Does NOT write the code (owned by frontend/backend)
- ❌ Does NOT merge PRs (owned by infrastructure-maintainer)
- ❌ Does NOT define coding standards (owned by tech lead/architect)
- ❌ Does NOT prioritize what gets built (owned by product)
