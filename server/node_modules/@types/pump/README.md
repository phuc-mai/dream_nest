# Installation
> `npm install --save @types/pump`

# Summary
This package contains type definitions for pump (https://github.com/mafintosh/pump).

# Details
Files were exported from https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/pump.
## [index.d.ts](https://github.com/DefinitelyTyped/DefinitelyTyped/tree/master/types/pump/index.d.ts)
````ts
/// <reference types="node" />

declare function pump(streams: pump.Stream[], callback?: pump.Callback): pump.Stream;

// callback have to be passed as last argument
declare function pump(...streams: Array<pump.Stream | pump.Callback>): pump.Stream;

declare namespace pump {
    type Callback = (err?: Error) => any;
    type Stream = NodeJS.ReadableStream | NodeJS.WritableStream;
}

export = pump;

````

### Additional Details
 * Last updated: Tue, 07 Nov 2023 09:09:39 GMT
 * Dependencies: [@types/node](https://npmjs.com/package/@types/node)

# Credits
These definitions were written by [Tomek Łaziuk](https://github.com/tlaziuk), and [Jason Cordial](https://github.com/jcordial).
