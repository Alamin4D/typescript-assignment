# Why `any` is a Type Safety Hole and Why `unknown` is Safer (with Type Narrowing)

## Introduction

TypeScript-এর মূল উদ্দেশ্য হলো type safety নিশ্চিত করা। কিন্তু `any` টাইপ এই safety system কে bypass করে ফেলে, যার কারণে এটিকে “type safety hole” বলা হয়। অন্যদিকে `unknown` টাইপ নিরাপদভাবে dynamic data handle করতে সাহায্য করে।

---

## Why `any` is Dangerous

`any` ব্যবহার করলে TypeScript কোনো ধরনের type checking করে না। এতে runtime error হওয়ার সম্ভাবনা অনেক বেড়ে যায়।

### Example:

```ts
let data: any;

data = "Hello";
data.toFixed(); // ❌ runtime error (string এ toFixed নেই)