# React Router Dom v6 Catch All Route '*' Not Working Correctly

This repository demonstrates a common issue encountered when using the catch-all route ('*') in React Router Dom v6.  The issue arises when nested routes are used and the catch-all route fails to catch paths that don't match any other defined routes. This example shows a simple implementation and steps to resolve the issue.

## Problem:

The catch-all route (`path="*"`) in React Router v6 should ideally capture any URL that doesn't match previously defined routes. However, in the presence of nested routes, it may fail to work as expected leading to unexpected behavior.

## Solution:

The catch-all route needs to be placed as the last route in the `Routes` component. This ensures that it only matches routes after all other routes have been checked.  The solution will demonstrate this fix.