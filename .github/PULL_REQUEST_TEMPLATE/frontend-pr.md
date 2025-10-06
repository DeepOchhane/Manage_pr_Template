## Description
Brief description of the changes made.

## Type of Change
- [ ] Bug fix (non-breaking change which fixes an issue)
- [ ] New feature (non-breaking change which adds functionality)
- [ ] Breaking change (fix or feature that would cause existing functionality to not work as expected)
- [ ] UI/UX improvement
- [ ] Performance improvement
- [ ] Code refactoring

## Effects Sanity Check
- [ ] If I added an effect, it connects React to an external system (network, storage, timers, subscriptions, DOM imperative work)
- [ ] This logic could not be handled at the **event boundary** (e.g., onOpenChange, router action)
- [ ] For data fetching I used **React Query/SWR** with enabled/queryKey instead of manual effects
- [ ] I did **not** mirror props to local state. Any computed value is derived (useMemo/variable), not synced
- [ ] I am **not** using useLayoutEffect (or this file is in the allowed folder for measurement/focus)
- [ ] Dependency arrays are minimal and stable (no unstable function identities unless memoized for a reason)

## Notes for Reviewers
**Why an effect is necessary here:**
<!-- Brief justification, e.g., "WebSocket subscribe/unsubscribe", "DOM measurement for positioning", etc. -->

## Frontend Testing
- [ ] I have tested these changes in the browser
- [ ] I have tested responsive behavior on different screen sizes
- [ ] I have tested keyboard navigation and accessibility
- [ ] I have tested in different browsers (Chrome, Firefox, Safari)
- [ ] New and existing tests pass locally

## Visual Changes
<!-- Add screenshots or GIFs if applicable -->

## Checklist
- [ ] My code follows the style guidelines of this project
- [ ] I have performed a self-review of my own code
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] My changes generate no new warnings
- [ ] I have updated component prop types/interfaces if needed

## Additional Notes
Any additional information, context, or performance considerations for reviewers.
