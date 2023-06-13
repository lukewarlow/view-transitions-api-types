# View Transitions API Types

[![npm](https://img.shields.io/npm/v/view-transitions-api-types.svg?style=flat-square)](https://www.npmjs.com/package/view-transitions-api-types)

Type definition for [`View Transitions API`](https://developer.mozilla.org/en-US/docs/Web/API/View_Transitions_API)

### Install

```shell
$ npm i -D view-transitions-api-types
```
### Usage

#### Make types visible in specific files

Add a [TypesScript triple-slash directive](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-types-)
as follows in any code-containing '.ts' file you want these types to be available in:

```typescript
// Add types for document.startViewTransition for use in this file. See https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-types- for more info.
/// <reference types="view-transitions-api-types" />

console.log(document.startViewTransition) // no type error!
```

#### Make types visible globally in all source files within a project

Create a `.d.ts` file anywhere in your project so that it is visible to TypeScript according to your `tsconfig.json` settings. For
example, it could be at `src/global.d.ts` or `src/view-transitions-api-types.d.ts`.

Add a [TypesScript triple-slash directive](https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-types-) as follows:

```typescript
// Add types for document.startViewTransition ambiently for implicit use in the entire project. See https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html#-reference-types- for more info.
/// <reference types="view-transitions-api-types" />
```

This exposes the types *ambiently* so they are available without any `import` or `require` statements. TypeScript will simply know about them everywhere.

**Important**: do not add any `import` or `export` statements to this file, or it will stop working ambiently. Doing that
changes it in TypeScript's view from a "script" to a "module", and the rules about ambient types change in that case.

## License

This project is licensed under the [MIT License](https://github.com/lukewarlow/view-transitions-api-types/blob/master/LICENSE).
