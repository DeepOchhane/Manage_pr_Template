# [JIRA-XXX] Brief descriptive title

## 🎯 What & Why

<!-- Concise description of what this PR accomplishes and why it's needed -->
<!-- Link to JIRA ticket, design spec, Figma, or related issue -->

**Closes:** #
**Related:** 
**Design:** [Figma/Design Link]

## ⚛️ React Effects Sanity Check

<!-- Complete this section if you added/modified useEffect, useLayoutEffect, or similar hooks -->

- [ ] **If I added an effect**, it connects React to an external system (network, storage, timers, subscriptions, DOM imperative work)
- [ ] **Event boundary check**: This logic could not be handled at the event boundary (e.g., `onOpenChange`, router action, form submission)
- [ ] **Data fetching**: For data fetching I used **React Query/SWR/TanStack Query** with `enabled`/`queryKey` instead of manual effects
- [ ] **State derivation**: I did **not** mirror props to local state. Any computed value is derived (`useMemo`/variable), not synced
- [ ] **Layout effects**: I am **not** using `useLayoutEffect` (or this file is in an allowed folder for measurement/focus/animation)
- [ ] **Dependencies**: Dependency arrays are minimal and stable (no unstable function identities unless memoized for a specific reason)

### ✍️ Effect Justification
<!-- Required if you added effects. Brief justification, e.g., "WebSocket subscribe/unsubscribe", "DOM measurement for tooltip positioning", "Keyboard event listener cleanup" -->

**Why an effect is necessary here:**

## 🧪 Frontend Testing & Validation

### Browser Testing
- [ ] ✅ Chrome (latest)
- [ ] ✅ Firefox (latest) 
- [ ] ✅ Safari (latest)
- [ ] ✅ Edge (latest)
- [ ] 📱 Mobile responsive (tested on device/dev tools)

### Accessibility & UX
- [ ] ⌨️ Keyboard navigation works correctly
- [ ] 🔍 Screen reader compatible (tested with dev tools)
- [ ] 🎨 Focus indicators are visible and appropriate
- [ ] 📏 WCAG contrast requirements met
- [ ] 🏷️ Semantic HTML elements used appropriately
- [ ] ⚡ Loading states implemented (if applicable)
- [ ] ❌ Error states handled gracefully

### Performance & Quality
- [ ] 🚀 No unnecessary re-renders (profiled with React DevTools)
- [ ] 💾 Bundle size impact considered (checked with bundler analysis)
- [ ] ⚡ Lazy loading implemented where appropriate
- [ ] 🖼️ Images optimized and responsive
- [ ] 📱 Works well on slow networks/devices

## 🔄 Type of Change

- [ ] 🐛 Bug fix (non-breaking change which fixes an issue)
- [ ] ✨ New feature (non-breaking change which adds functionality)
- [ ] 💥 Breaking change (fix or feature that causes existing functionality to break)
- [ ] 🎨 UI/UX improvement or design update
- [ ] ♿ Accessibility improvement
- [ ] ⚡ Performance optimization
- [ ] 🔧 Refactoring (no functional changes)

## 📸 Visual Changes

<!-- Include before/after screenshots, GIFs, or videos. Use tools like LICEcap for GIFs -->

### Desktop
<!-- Screenshots for desktop view -->

### Mobile  
<!-- Screenshots for mobile view -->

### Interactive Demo
<!-- Link to deployed preview, Storybook, or CodeSandbox if available -->

## 📋 Pre-Merge Checklist

### Code Quality
- [ ] My code follows the project's style guidelines (ESLint/Prettier passed)
- [ ] I have performed a self-review of my code
- [ ] I have commented complex/non-obvious code sections
- [ ] Component props have proper TypeScript types/PropTypes
- [ ] No console logs or debugging code left in

### Testing
- [ ] Unit tests added/updated for new functionality
- [ ] Component tests cover user interactions
- [ ] Integration tests pass (if applicable)
- [ ] Visual regression tests updated (if applicable)
- [ ] Tested with both dev and production builds

### Documentation & Standards
- [ ] Storybook stories added/updated (if applicable)
- [ ] Component documentation updated
- [ ] Props/API changes documented
- [ ] Design system compliance verified

### Performance & Security
- [ ] No memory leaks (effects properly cleaned up)
- [ ] No XSS vulnerabilities introduced
- [ ] Form validation implemented (client + server side)
- [ ] Sensitive data properly handled
- [ ] Analytics events implemented (if applicable)

## 🚨 Breaking Changes

<!-- If this introduces breaking changes, describe impact and migration path -->

## 🔗 Dependencies & Post-Merge Tasks

<!-- List any dependencies or follow-up tasks -->
- [ ] Requires backend API changes: 
- [ ] Design system updates needed: 
- [ ] Documentation site updates: 
- [ ] Analytics tracking updates: 
- [ ] Third-party integration updates: 

## 🎭 How does this make you feel?

<!-- Optional: Add a GIF that represents how this PR makes you feel or what it accomplishes -->
<!-- This can help make code reviews more engaging and fun! -->

## 📝 Additional Notes

<!-- Any additional context, architectural decisions, trade-offs, or concerns for reviewers -->
<!-- Include any performance metrics, lighthouse scores, or other relevant data -->
