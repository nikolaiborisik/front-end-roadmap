# 📝 TypeScript Fundamentals

## Table of Contents

- [Introduction and quick start](#Introduction-and-quick-start)
- [Topics to cover](#Topics-to-cover)
- [Optional](#Optional)
- [Exercises](#Exercises)
- [Tasks](#Tasks)
  - [Task 1](#Task-1)
  - [Task 2](#Task-2)
  - [Task 3](#Task-3)
  - [Task 4](#Task-4)
  - [Task 5](#Task-5)
  - [Task 6](#Task-6)

## Introduction and quick start

[TypeScript](https://www.typescriptlang.org/) is a superset of JavaScript language which benefits from type system to enable compile time type analysis. A valid JS code is a valid TS code too, but to run TS in a browser or any other environment, you need to transform TS into plain JS code. The easiest way to try TypeScript is to use [The Playground](https://www.typescriptlang.org/play). This would be sufficient enough to solve all the tasks on this step, but it is not something that will be useful in a real world. The next step would be to [add TypeScript to your workstation](https://www.typescriptlang.org/download) and add support for your favourite IDE (details [here](https://exploringjs.com/tackling-ts/ch_typescript-workflows.html#programming-typescript-via-an-integrated-development-environment-ide)). Keep in mind, that every feature comes with the price, so make sure to get familiar with [benefits](https://exploringjs.com/tackling-ts/ch_why-typescript.html#the-benefits-of-using-typescript) TypeScript grants developer as well as [downsides](https://exploringjs.com/tackling-ts/ch_why-typescript.html#the-downsides-of-using-typescript) such solution brings upon them.

This step is only an introduction to the world of TypeScript. See [the official documentation](https://www.typescriptlang.org/docs/) for extra and missing information.

## Topics to cover

- Type
  annotations [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#type-annotations) [link](https://www.typescriptlang.org/docs/handbook/2/basic-types.html#explicit-types)
- Primitive
  Types [link](https://basarat.gitbook.io/typescript/type-system#primitive-types) [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#the-primitives-string-number-and-boolean)
- Literal types [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#literal-types)
- null and
  undefined [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#by-default-undefined-and-null-are-not-included-in-types) [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#null-and-undefined)
- Arrays [link](https://basarat.gitbook.io/typescript/type-system#arrays) [link](https://exploringjs.com/tackling-ts/ch_typing-arrays.html#ways-of-typing-arrays)
- Array as tuples [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#arrays-as-tuples)
- Function
  types [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#function-types) [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#functions)
  - void [link](https://basarat.gitbook.io/typescript/type-system#any)
  - Optional parameters [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#optional-parameters)
  - Rest parameters [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#rest-parameters)
- Union types [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#union-types)
- Typing objects [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#typing-objects)

  - Typing objects-as-records via
    interfaces [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#typing-objects-as-records-via-interfaces)
  - Object literal
    types [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#object-literal-types)
  - Methods [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#methods)
  - Optional Properties [link](https://www.typescriptlang.org/docs/handbook/2/objects.html#optional-properties)
  - Readonly Properties [link](https://www.typescriptlang.org/docs/handbook/2/objects.html#readonly-properties)

- Enums
  - Numeric enums [link](https://exploringjs.com/tackling-ts/ch_enums.html#numeric-enums)
  - String-based enum [link](https://exploringjs.com/tackling-ts/ch_enums.html#string-based-enums)
  - Heterogeneous enums [link](https://exploringjs.com/tackling-ts/ch_enums.html#heterogeneous-enums)
  - Omitting initializers [link](https://exploringjs.com/tackling-ts/ch_enums.html#omitting-initializers)
- Do practical exercises: Task 1-4,E1-E2
- Generic Object
  Types [link](https://www.typescriptlang.org/docs/handbook/2/objects.html#generic-object-types) [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#type-variables-and-generic-types)
- Any [link](https://basarat.gitbook.io/typescript/type-system#any) [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#any) [examples](https://www.typescriptlang.org/play?q=183#example/any)
  - noImplicitAny [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#noimplicitany)
  - When to use
    any[link](https://github.com/formium/typescript#when-to-use-any)
- Utility Types [link](https://www.typescriptlang.org/docs/handbook/utility-types.html)
  - Partial<Type> [link](https://www.typescriptlang.org/docs/handbook/utility-types.html#partialtype)
  - Record<Keys,Type> [link](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeystype)
- Structural
  typing [link](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html#structural-type-system)
- Static
  type-checking [link](https://en.wikipedia.org/wiki/Type_system#Static_type_checking) [link](https://en.wikipedia.org/wiki/Type_system#Dynamic_type_checking_and_runtime_type_information)
- Type Inference [link](https://www.typescriptlang.org/docs/handbook/type-inference.html)
- Type Assertions [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#type-assertions)
- Type guards
  - Built-in type
    guards [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#narrowing-via-built-in-type-guards) [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#when-are-static-types-too-general)
  - User-defined type
    guards [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#user-defined-type-guards)

## Optional

### TypeScript and React Fundamentals [link](react.md#Fundamentals)

## Exercises

For exercises use WebStorm or VSCode or TSPlayground. For WebStorm and VSCode create an empty project and add a .ts file, TypeScript should work out of the box.

### From typescript-exercises [link](https://github.com/typescript-exercises/typescript-exercises/)

Fork repo https://github.com/typescript-exercises/typescript-exercises/
. [How to fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo)

- [E1](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/1) Interface, Array
- [E2](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/2) Union
- [E3](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/3) Built-in type guards
- [E4](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/4) User-defined type guards
- [E5](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/5) Utility types
- [E7](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/7) Generic, Function,
  Tuples
- [E9](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/9) Generic

## Tasks

- Create repo in the GitHub.
- Send link to your mentor
- For each task create ts file task#.ts.

### Task 1

Describe interface User that has the following properties: id, firstName, lastName, isOnline, age, role, address. See
usage example below

```typescript
const user1: User = {
  id: "111",
  firstName: "Ivan",
  lastName: "Ivanov",
  isOnline: false,
  age: 20,
  role: "user",
  address: {
    city: "Minsk",
    country: "Belarus",
    zip: "220000",
  },
};

const user2: User = {
  id: "222",
  firstName: "Ivan",
  lastName: "Ivanov",
  isOnline: false,
  age: 20,
  role: "user",
  address: null,
};

const user3 = {
  id: "333",
  firstName: "Ivan",
  lastName: "Ivanov",
  isOnline: false,
  role: "user",
  address: null,
};
```

### Task 2

Define the following types `Role` (use enum), `Feature` (use union), `Permissions`, `FeaturePermission`. Available roles
are guest, user, and admin. Available features are catalog, basket, news, report. Available permissions are `NO_ACCESS`
, `READ`, `READ_WRITE`. For type `FeaturePermission` use utility types Record and Partial.

```typescript
// TODO: define Role, Feature, Permission and FeaturePermission

let role: Role = Role.Guest;

let feature: Feature = "catalog";
let permission: Permission = "READ";
const permissions: FeaturePermission = {
  guest: {
    catalog: "READ",
    news: "READ",
  },
  user: {
    catalog: "READ",
    basket: "READ_WRITE",
    news: "READ",
  },
  admin: {
    catalog: "READ_WRITE",
    news: "READ",
    report: "READ",
  },
};
```

### Task 3

Type function hasPermission. See example for more details

```js
function hasAccess(user, features) {
  const role = user.role;
  const rolePermissions = permissions[role];
  const featuresToCheck = Array.isArray(features) ? features : [features];
  return featuresToCheck.every((feature) =>
    ["READ", "READ_WRITE"].includes(rolePermissions[feature])
  );
}

const hasAccessToCatalog = hasAccess(user, "catalog");
const hasAccessToCatalogAndBasket = hasAccess(user, ["basket", "catalog"]);
```

### Task 4

Type function updateUser. See js example for more details below.

```js
function updateUser(user, newValues) {
  return { ...user, ...newValues };
}

const updatedUser = updateUser(user, { isOnline: true });
const updatedUser2 = updateUser(user, { age: 25, lastName: "Petrov" });
```

### Task 5

Type function `useState`. See source code for more details

```js
function useState(initialValue) {
  let currentValue = initialValue;
  const setValue = (value) => {
    currentValue = value;
  };
  const getValue = () => currentValue;
  return [getValue, setValue, initialValue];
}

const [getValue, setValue, initialValue] = useState(10);
const v = getValue();
setValue(20);
```

### Task 6

Create interface Array<T> with following arrays method: pop, push, sort, indexOf, every, map, filter, reduce. Use
javascript docs as
references. [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
Example for [slice](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice#syntax)
method

```typescript
interface Array<T> {
  slice(start?: number, end?: number): T[];
}
```
