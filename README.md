# Shopify Theme Developer Assessment

## Overview

This assessment contains **two tests** to evaluate your Shopify theme development skills. Please complete both tests and submit as a single Pull Request.

**Total Time**: 60-75 minutes
- Test 1 (Build): ~45 minutes
- Test 2 (Debug): ~20 minutes

---

## Submission Instructions

1. Fork this repository
2. Create a new branch named `assessment/[your-name]`
3. Complete both tests
4. Submit a Pull Request to the main repository
5. PR title format: `Assessment Submission - [Your Name]`

> ⏱️ Your submission time will be recorded via the PR timestamp.

---

## Test 1: Build a Team Members Section

### Objective

Create a team members section that displays staff profiles from a metaobject.

### File to Create

```
sections/team-members.liquid
```

### What to Display (per team member)

- Photo
- Name  
- Job title
- Short bio (optional — merchant should be able to hide this)
- LinkedIn link (optional)

### Section Controls

The merchant should be able to customize:
- Section heading and subheading
- Toggle bio visibility on/off
- Colors

### Layout Requirements

| Viewport | Behavior |
|----------|----------|
| **Mobile** (< 768px) | Horizontal slider using CSS scroll-snap |
| **Tablet** (768px – 1024px) | 2×2 grid |
| **Desktop** (> 1024px) | Auto-fit grid that expands with screen width |

### Technical Requirements

- [ ] Pull data from a `team_member` metaobject (assume it exists)
- [ ] Use `{% liquid %}` blocks for Liquid logic
- [ ] All schema settings must have sensible default values
- [ ] SEO-compliant HTML structure (proper heading hierarchy, semantic elements)
- [ ] Accessible markup (alt text, ARIA where needed, keyboard navigable slider)
- [ ] BEM class naming convention
- [ ] Handle empty state (no metaobject list selected)

## Test 2: Debug the Liquid Section With Errors

### Objective

The file `file-with-issues.liquid` contains errors please find and fix all of them.

### File to Fix

```
file-with-issues.liquid
```

### How to Document Your Fixes

Add a comment above each fix explaining what was wrong:

```liquid
{%- comment -%} FIX #1: Description of what was wrong and why {%- endcomment -%}
```

## What We're Looking For

### ✅ Do

- Write clean, maintainable code
- Use semantic HTML elements
- Follow BEM naming conventions
- Include sensible default values
- Handle edge cases (empty states)
- Write accessible markup

### ❌ Don't

- Over-engineer the solution
- Use external libraries/dependencies
- Leave console errors or invalid JSON
- Skip accessibility considerations

---

## Questions?

If anything is unclear, make a reasonable assumption and note it in your PR description.

Good luck! 🚀
