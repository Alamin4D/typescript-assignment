# How Generics Help Build Reusable and Strictly Typed Components in TypeScript

## Introduction

Generics TypeScript-এর একটি powerful feature, যা আমাদেরকে reusable এবং strongly typed function/component তৈরি করতে সাহায্য করে।

---

## Problem Without Generics

Generics ছাড়া আমাদের আলাদা আলাদা function লিখতে হয় বিভিন্ন data type এর জন্য, যা code duplication তৈরি করে।

### Example:

```ts
function getFirstNumber(arr: number[]): number {
  return arr[0];
}

function getFirstString(arr: string[]): string {
  return arr[0];
}