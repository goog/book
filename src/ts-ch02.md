下面是一份**TypeScript 基础类型 + 组合类型学习课程（Markdown版）**，适合入门学习，也适合当复习资料使用。

---

# TypeScript 基础类型与组合类型教程

TypeScript 是 JavaScript 的超集，它在 JS 基础上增加了**静态类型系统**，可以在编译阶段发现错误，提高代码可维护性。

---

# 一、基础类型（Basic Types）

## 1. number（数字类型）

```ts
let age: number = 18;
let price: number = 99.99;
```

👉 支持整数和浮点数，没有区分 int/float

---

## 2. string（字符串）

```ts
let name: string = "Alice";
let message: string = `Hello, ${name}`;
```

---

## 3. boolean（布尔类型）

```ts
let isLogin: boolean = true;
let isDeleted: boolean = false;
```

---

## 4. null 和 undefined

```ts
let n: null = null;
let u: undefined = undefined;
```

👉 通常用于“值不存在”

---

## 5. any（任意类型）

```ts
let data: any = 123;
data = "hello";
data = true;
```

⚠️ 不推荐使用，会失去类型检查优势

---

## 6. unknown（未知类型）

```ts
let value: unknown = "hello";

// 必须进行类型判断才能使用
if (typeof value === "string") {
  console.log(value.toUpperCase());
}
```

👉 比 any 更安全

---

## 7. void（无返回值）

```ts
function logMessage(): void {
  console.log("Hello TypeScript");
}
```

---

## 8. never（永不存在的值）

```ts
function throwError(): never {
  throw new Error("Error!");
}
```

👉 常用于报错函数或死循环

---

# 二、数组类型（Array）

## 1. 基本写法

```ts
let nums: number[] = [1, 2, 3];
let names: string[] = ["Alice", "Bob"];
```

---

## 2. 泛型写法

```ts
let nums: Array<number> = [1, 2, 3];
```

---

# 三、元组类型（Tuple）

👉 固定长度 + 固定类型

```ts
let user: [string, number] = ["Alice", 18];
```

访问：

```ts
console.log(user[0]); // string
console.log(user[1]); // number
```

每个位置类型可以不同，但顺序固定长度固定的数组

---

# 四、对象类型（Object）

```ts
let person: {
  name: string;
  age: number;
} = {
  name: "Alice",
  age: 18,
};
```

---

# 五、函数类型

## 1. 基本函数

```ts
function add(a: number, b: number): number {
  return a + b;
}
```

---

## 2. 箭头函数

```ts
const multiply = (a: number, b: number): number => {
  return a * b;
};
```

---

## 3. 函数类型声明

```ts
let fn: (x: number, y: number) => number;

fn = (a, b) => a + b;
```

---

# 六、联合类型（Union Types）

👉 多种类型之一

```ts
let id: number | string;

id = 123;
id = "abc";
```

---

## 实战示例

```ts
function printId(id: number | string) {
  console.log("ID:", id);
}
```

---

# 七、交叉类型（Intersection Types）

👉 多种类型合并

```ts
type A = {
  name: string;
};

type B = {
  age: number;
};

type C = A & B;

let person: C = {
  name: "Alice",
  age: 18,
};
```

---

# 八、字面量类型（Literal Types）

```ts
let direction: "left" | "right";

direction = "left";
// direction = "up"; ❌ 错误
```

---

# 九、类型别名（Type Alias）

```ts
type UserID = string | number;

let id: UserID = 123;
```

---

# 十、接口（Interface）

```ts
interface User {
  name: string;
  age: number;
}

const user: User = {
  name: "Alice",
  age: 18,
};
```

---

## interface vs type

|特性|interface|type|
|---|---|---|
|扩展|支持 extends|支持 &|
|推荐|对象结构|更灵活|

---

# 十一、可选属性（Optional Properties）

```ts
interface User {
  name: string;
  age?: number;
}
```

---

# 十二、只读属性（readonly）

```ts
interface User {
  readonly id: number;
  name: string;
}

const user: User = {
  id: 1,
  name: "Alice",
};

// user.id = 2 ❌ 错误
```

---

# 十三、综合示例（实战）

```ts
type Role = "admin" | "user";

interface Account {
  id: number;
  name: string;
  role: Role;
}

function login(account: Account): string {
  if (account.role === "admin") {
    return "Welcome Admin";
  }
  return "Welcome User";
}
```

---

# 总结

TypeScript 类型系统核心可以归纳为：

- 基础类型：number / string / boolean
    
- 特殊类型：any / unknown / void / never
    
- 组合类型：union / intersection
    
- 结构类型：interface / type
    
- 扩展能力：tuple / literal / optional / readonly
    

