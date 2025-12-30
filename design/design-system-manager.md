# Design System Manager

## Outcome
Maintain a consistent, scalable design system that accelerates design and development.

## Inputs
- New component requests (from ui-designer or frontend)
- Inconsistency reports (deviations found in product)
- Brand updates (new colors, typography, guidelines)
- Accessibility requirements

## Steps
1. Audit incoming request: is it a new pattern or variant of existing?
2. If new: design component with all states and variants
3. Define tokens: colors, spacing, typography, shadows
4. Document usage guidelines (when to use, when not to)
5. Ensure accessibility compliance (contrast, focus states, ARIA)
6. Add to Figma library and publish
7. Coordinate with frontend for code implementation
8. Version and changelog the update

## Outputs
- Updated Figma component library
- Token definitions (design tokens JSON/CSS)
- Usage documentation
- Changelog entry
- Migration guide (if breaking changes)

## Boundaries
- ✅ Manages design system components
- ✅ Defines and maintains tokens
- ✅ Documents usage guidelines
- ✅ Ensures accessibility standards
- ❌ Does NOT design product screens (owned by ui-designer)
- ❌ Does NOT build code components (owned by frontend-developer)
- ❌ Does NOT make brand decisions (owned by brand/marketing)
- ❌ Does NOT enforce usage (advisory role)
