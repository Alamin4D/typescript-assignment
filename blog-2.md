# How Generics Help Build Reusable and Strictly Typed Components in TypeScript

## 📌 Introduction

Generics are a powerful feature of TypeScript that help us create **reusable** and **strongly typed** functions or components.

---

## ❌ Problem Without Generics

Without generics, we need to write separate functions for different data types, which leads to **code duplication** and makes the code harder to maintain.

### ❌ Example:

```ts
function getFirstNumber(arr: number[]): number {
  return arr[0];
}

function getFirstString(arr: string[]): string {
  return arr[0];
}
```

### ⚠️ Problem:

* Code duplication
* Hard to maintain
* Poor scalability

---

## ✅ Solution: Using Generics

With generics, we can handle multiple data types using a single function.

---

## 🔥 Generic Example:

```ts
function getFirstElement<T>(arr: T[]): T {
  return arr[0];
}
```

---

## 🧪 Usage Example:

```ts
console.log(getFirstElement<number>([1, 2, 3]));
console.log(getFirstElement<string>(["a", "b", "c"]));
```

---

## 🎯 Benefits of Generics

* ✔ Code reusability increases
* ✔ Strong type safety
* ✔ Reduces duplication
* ✔ More scalable and maintainable code

---
