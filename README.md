# Tailwind CSS Dynamic Content Issue in Next.js/Nuxt.js

This repository demonstrates a common bug encountered when using Tailwind CSS with Next.js or Nuxt.js.  The problem occurs when dynamically rendered content doesn't pick up Tailwind classes, resulting in unstyled elements.  This is typically caused by issues with Tailwind's JIT (Just-In-Time) compilation mode.

## Problem

The `bug.js` file contains a Next.js component that renders a list of items. Each list item should have Tailwind classes applied (`bg-blue-500`, `p-4`, `rounded`), but they are not applied correctly due to a misconfiguration in how Tailwind's JIT compilation is handled in the build process.

## Solution

The `bugSolution.js` file shows the corrected approach. The key changes are shown in the comments of that file.  Generally, this often involves ensuring Tailwind's configuration is properly set up to support dynamic class generation within your framework's build process.