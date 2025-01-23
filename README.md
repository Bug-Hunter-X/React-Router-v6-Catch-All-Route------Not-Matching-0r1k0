# React Router v6 Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6.  Routes defined before the catch-all route are correctly matched, but the catch-all route fails to handle unmatched paths.

## Problem
The issue occurs when using `Routes` and `Route` components.  If a route with a specific path is defined before a catch-all route, the catch-all route is never reached, even for invalid paths.

## Solution
The solution involves placing the catch-all route as the last route in the `Routes` component.  This ensures that it is the final fallback for any unmatched paths.