---
title: Http/Headers.ts
nav_order: 13
parent: "@effect/platform"
---

## Headers overview

Added in v1.0.0

---

<h2 class="text-delta">Table of contents</h2>

- [combinators](#combinators)
  - [remove](#remove)
  - [set](#set)
  - [setAll](#setall)
- [constructors](#constructors)
  - [empty](#empty)
  - [fromInput](#frominput)
- [models](#models)
  - [Headers (interface)](#headers-interface)
  - [Input (type alias)](#input-type-alias)

---

# combinators

## remove

**Signature**

```ts
export declare const remove: ((key: string) => (self: Headers) => Headers) & ((self: Headers, key: string) => Headers)
```

Added in v1.0.0

## set

**Signature**

```ts
export declare const set: ((key: string, value: string) => (self: Headers) => Headers) &
  ((self: Headers, key: string, value: string) => Headers)
```

Added in v1.0.0

## setAll

**Signature**

```ts
export declare const setAll: ((headers: Input) => (self: Headers) => Headers) &
  ((self: Headers, headers: Input) => Headers)
```

Added in v1.0.0

# constructors

## empty

**Signature**

```ts
export declare const empty: Headers
```

Added in v1.0.0

## fromInput

**Signature**

```ts
export declare const fromInput: (input?: Input) => Headers
```

Added in v1.0.0

# models

## Headers (interface)

**Signature**

```ts
export interface Headers extends HashMap.HashMap<string, string> {}
```

Added in v1.0.0

## Input (type alias)

**Signature**

```ts
export type Input = Headers | Readonly<Record<string, string>> | Iterable<readonly [string, string]>
```

Added in v1.0.0
