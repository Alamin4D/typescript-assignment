# Why `any` is a Type Safety Hole and Why `unknown` is Safer (with Type Narrowing)

## Introduction

The main purpose of TypeScript is to ensure type safety. However, the any type bypasses this safety system, which is why it is called a “type safety hole.” On the other hand, the unknown type helps handle dynamic data safely.

---

## Why `any` is Dangerous

When using any, TypeScript does not perform any type checking. As a result, the chances of runtime errors increase significantly.

### Example:

```ts
let data: any;

data = "Hello";
data.toFixed(); // ❌ runtime error (toFixed does not exist on the string type)