# Typescript
Topic Leaders: 
- 
## Fundamentals

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
  - Typing objects-as-records via interfaces [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#typing-objects-as-records-via-interfaces))
  - Object literal types [link](https://exploringjs.com/tackling-ts/ch_typescript-essentials.html#object-literal-types)
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
  - Built-in type guards [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#narrowing-via-built-in-type-guards) [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#when-are-static-types-too-general)
- The benefits of using TypeScript [link](https://exploringjs.com/tackling-ts/ch_why-typescript.html#the-benefits-of-using-typescript)
- The downsides of using TypeScript [link](https://exploringjs.com/tackling-ts/ch_why-typescript.html#the-downsides-of-using-typescript)

### Exercises
[1](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/1)
[2](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/2)
[3](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/3)
[7](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/7)
[9](https://github.com/typescript-exercises/typescript-exercises/tree/master/src/exercises/9)



## Intermediate
- Keyof Type Operator [link](https://www.typescriptlang.org/docs/handbook/2/keyof-types.html)
- Typeof Type Operator [link](https://www.typescriptlang.org/docs/handbook/2/typeof-types.html)
- Utility Types  [link](https://www.typescriptlang.org/docs/handbook/utility-types.html)
  - Required<Type> 
  - Pick<Type, Keys>
  - Omit<Type, Keys> 
  - Exclude<Type, ExcludedUnion> 
  - Extract<Type, Union>
  - NonNullable<Type>
  - Parameters<Type>
  - ConstructorParameters<Type>
  - ReturnType<Type>
  - InstanceType<Type>
  - ThisParameterType<Type>
  - OmitThisParameter<Type> 
  - ThisType<Type>
- Never Type [link](https://basarat.gitbook.io/typescript/type-system/never)    
-  type unknown [link](https://exploringjs.com/tackling-ts/ch_any-unknown.html#the-top-type-unknown)
- Enum 
  - Literal enum members  [link](https://exploringjs.com/tackling-ts/ch_enums.html#literal-enum-members)
  - Constant enum members [link](https://exploringjs.com/tackling-ts/ch_enums.html#constant-enum-members)
  - Computed enum members [link](https://exploringjs.com/tackling-ts/ch_enums.html#computed-enum-members)
  - Use cases for enums [link](https://exploringjs.com/tackling-ts/ch_enums.html#use-cases-for-enums)
- Typing Arrays [link](https://exploringjs.com/tackling-ts/ch_typing-arrays.html) 
- Freshness [link](https://basarat.gitbook.io/typescript/type-system/freshness)
- Type guards
  - User-defined type guards [link](https://exploringjs.com/tackling-ts/ch_type-guards-assertion-functions.html#user-defined-type-guards)
- Typing functions  [link](https://exploringjs.com/tackling-ts/ch_typing-functions.html)
- Indexed Access Types [link](https://www.typescriptlang.org/docs/handbook/2/indexed-access-types.html)

## Advance
- Enum
  - Enums at runtime [link](https://exploringjs.com/tackling-ts/ch_enums.html#enums-at-runtime)
  - const enums [link](https://exploringjs.com/tackling-ts/ch_enums.html#const-enums)
  - Enums at compile time [link](https://exploringjs.com/tackling-ts/ch_enums.html#enums-at-compile-time)
- Unions of singleton values [link](https://exploringjs.com/tackling-ts/ch_enum-alternatives.html#unions-of-singleton-values)
- Discriminated unions [link](https://exploringjs.com/tackling-ts/ch_enum-alternatives.html#discriminated-union) [link](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes-func.html#discriminated-unions)
- Object literals as enums  [link](https://exploringjs.com/tackling-ts/ch_enum-alternatives.html#object-literals-as-enums)

  
- Conditional Types [link](https://www.typescriptlang.org/docs/handbook/2/conditional-types.html)
- Mapped Types [link](https://www.typescriptlang.org/docs/handbook/2/mapped-types.html)
- Template Literal Types [link](https://www.typescriptlang.org/docs/handbook/2/template-literal-types.html)
  - Intrinsic String Manipulation Types [link](https://www.typescriptlang.org/docs/handbook/utility-types.html#intrinsic-string-manipulation-types)
- Namespaces  [link](https://www.typescriptlang.org/docs/handbook/namespaces.html)
- Nominal Typing [link](https://basarat.gitbook.io/typescript/main-1/nominaltyping)


## Links

### Books and guides

- [basarat.gitbook.io](https://basarat.gitbook.io/typescript/)
- [The TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html) - Official handbook
- [Tackling TypeScript](https://exploringjs.com/tackling-ts/toc.html)

### Others

- [Language developing roadmap](https://github.com/microsoft/TypeScript/wiki/Roadmap) This page outlines specific features and fixes that are scheduled or planned for given releases.
- [TypeScript Design Goals](https://github.com/microsoft/TypeScript/wiki/TypeScript-Design-Goals)
- [TypeScript FAQ](https://github.com/microsoft/TypeScript/wiki/FAQ)

### Exercises

- [Type challenges](https://github.com/type-challenges/type-challenges) - Collection of TypeScript type challenges
- [typescript-exercises](https://github.com/typescript-exercises/typescript-exercises) 
- [Advanced TypeScript Exercises](https://dev.to/macsikora/advanced-typescript-exercises-question-1-45k4)
