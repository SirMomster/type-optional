# type-optional 

The bare minimum for an optional type in TypeScript. This is just a type nothing more and nothing less.

## Usage

Use the type as followed:

```ts
import { Optional, OptionalPromise } from "type-optional";
// Use OptionalPromise for async functions

function test(): Optional<string> {
    return "test";
}

function otherTest(test: string) {
    // something
}

otherTest(test()); // Argument of type 'Optional<string>' is not assignable to parameter of type 'string'. Type 'undefined' is not assignable to type 'string'
```

## Todo

- Include some utility functions?