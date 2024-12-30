# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug causes an infinite loop due to improper usage of the dependency array.

## Bug Description

The `useEffect` hook, when used without a dependency array or with an incorrect dependency array, can trigger an infinite loop. In this example, the component renders continuously because the effect's dependency array is missing. This leads to an infinite loop and performance issues. 

## Bug Solution

The solution is to include the `count` variable in the dependency array of `useEffect` to make the effect runs only when `count` changes.