# Next.js 15 Janky Page Transitions

This repo demonstrates a janky page transition issue in a simple Next.js 15 app.  Navigation between pages works, but the transition is not smooth; there's a noticeable flicker or jump.

## Problem Description

The app has two pages: a home page (`/`) and an about page (`/about`).  Clicking links to navigate between pages should provide a smooth transition.  However, a jarring, unpolished transition occurs.

## Solution

The solution involves adding the `prefetch` prop to the `<Link>` component in `pages/index.js`. This prefetches the about page resources in the background, making the transition significantly smoother.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate between the Home and About pages by clicking the link.
5. Observe the janky page transitions.
6. Apply the solution to see the improvement.