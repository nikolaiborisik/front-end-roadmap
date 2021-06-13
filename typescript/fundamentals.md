# TypeScript Fundamentals

- Static type-checking [link](https://www.typescriptlang.org/docs/handbook/2/basic-types.html#static-type-checking)
- Type annotations [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#type-annotations)
- Primitive Types [link](https://basarat.gitbook.io/typescript/type-system#primitive-types)
- null and undefined [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#union-types)
- Arrays [link](https://basarat.gitbook.io/typescript/type-system#arrays) [link](https://basarat.gitbook.io/typescript/type-system#arrays)
- Array as tuples [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#arrays-as-tuples)
- Function types [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#function-types)
  - void [link](https://basarat.gitbook.io/typescript/type-system#any)
- Union types [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#union-types)
- Typing objects [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#typing-objects)
  - Typing objects-as-records via
    interfaces [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#typing-objects-as-records-via-interfaces)
  - Object literal
    types [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#object-literal-types)
  - Methods [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#methods)
  - Optional Properties [link](https://www.typescriptlang.org/docs/handbook/2/objects.html#optional-properties)
  - Readonly Properties [link](https://www.typescriptlang.org/docs/handbook/2/objects.html#readonly-properties)
  - Generic Object Types [link](https://www.typescriptlang.org/docs/handbook/2/objects.html#generic-object-types)
- Any [link](https://basarat.gitbook.io/typescript/type-system#any)
- Enums
  - Numeric enums [link](https://exploringjs.com/tackling-ts/ch_enums.html#numeric-enums)
  - String-based enum [link](https://exploringjs.com/tackling-ts/ch_enums.html#string-based-enums)
  - Heterogeneous enums [link](https://exploringjs.com/tackling-ts/ch_enums.html#heterogeneous-enums)
  - Omitting initializers [link](https://exploringjs.com/tackling-ts/ch_enums.html#omitting-initializers)
- Utility Types [link](https://www.typescriptlang.org/docs/handbook/utility-types.html)
  - Partial<Type> [link](https://www.typescriptlang.org/docs/handbook/utility-types.html#partialtype)
  - Record<Keys,Type> [link](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeystype)
- Type Inference [link](https://www.typescriptlang.org/docs/handbook/type-inference.html)
- Type Assertions [link](https://www.typescriptlang.org/docs/handbook/2/everyday-types.html#type-assertions)
- Type guards
  - Built-in type
    guards [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#narrowing-via-built-in-type-guards) [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#when-are-static-types-too-general)
- The benefits of using
  TypeScript [link](https://exploringjs.com/tackling-ts/ch_why-typescript.html#the-benefits-of-using-typescript)
- The downsides of using
  TypeScript [link](https://exploringjs.com/tackling-ts/ch_why-typescript.html#the-downsides-of-using-typescript)

## Exercises

From [typescript-exercises](https://github.com/typescript-exercises/typescript-exercises/):
[1](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/1)
[2](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/2)
[3](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/3)
[7](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/7)
[9](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/9)

## Tasks

### Task 1

Describe type User that have following properties: id, firstName, lastName, isOnline, age, role, address.
See example for more details

```js
const user1 = {
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

const user2 = {
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

Type function updateUser. See example for more details.

```js
function updateUser(user, newValues) {
  return { ...user, ...newValues };
}
const updatedUser = updateUser(user, { isOnline: true });
const updatedUser2 = updateUser(user, { age: 25, lastName: "Petrov" });
```

### Task 3

Define following types Role (use enum), Feature (use union), FeaturePermission, Permissions
Available
roles are guest, user and admin. Available features are catalog, basket, admin, report. Available permissions are
NO_ACCESS, READ, READ_WRITE'

```typescript
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

### Task 4

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

### Task 5

Type function `useState`. See source code for more details

```js
function useState(initialValue) {
  const currentValue = initialValue;
  const setValue = (value) => {
    currentValue = initialValue;
  };
  const getValue = () => currentValue;
  return [getValue, setValue, initialValue];
}

const [getValue, setValue, initialValue] = useState(10);
const v = getValue();
setValue(20);
```

### Task 5

Create interface Array<T> with following arrays method: pop, push, sort, indexOf, every, map, filter,
reduce. Use javascript docs as references. [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
