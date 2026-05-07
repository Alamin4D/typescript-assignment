# 🚨 Why `any` is a Type Safety Hole and Why `unknown` is Safer in TypeScript

## 📌 Introduction

TypeScript is designed to provide **type safety** and reduce runtime errors. However, not all types follow this safety system strictly. One such example is the `any` type, which completely bypasses TypeScript’s type checking.

On the other hand, the `unknown` type provides flexibility but still keeps your code safe by forcing type checking before use.

---

## ❌ Why `any` is Dangerous

The `any` type disables TypeScript’s type system. Once a variable is declared as `any`, you can perform any operation on it without errors during compile time.

### ❌ Example:

```ts
let data: any;

data = "Hello";
data.toFixed(); // ❌ Runtime error
```

### ⚠️ Key Problems:

* No type checking
* Unsafe operations allowed
* Errors only appear at runtime

---

## ✅ Why `unknown` is Safer

The `unknown` type also accepts any value, but it does not allow direct usage without type checking.

This means TypeScript forces you to verify the type before performing any operation.

---

### 🔍 Example:

```ts
let data: unknown;

data = "Hello";

// data.toUpperCase(); ❌ Error: Object is of type 'unknown'

if (typeof data === "string") {
    console.log(data.toUpperCase()); // ✅ Safe
}
```