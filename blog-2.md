# How Generics Help Build Reusable and Strictly Typed Components in TypeScript

## Introduction

Generics are a powerful feature of TypeScript that help us create reusable and strongly typed functions and components.

---

## Problem Without Generics

Without generics, we need to write separate functions for different data types, which leads to code duplication.

### Example:

```ts
function getFirstNumber(arr: number[]): number {
  return arr[0];
}

function getFirstString(arr: string[]): string {
  return arr[0];
}