# Typescript

## Benefits of using typeScript

-Static Typing
-Code Completion
-Refactoring
-Shorthand notations
-Using new javascript feaytures that javascript browsers haven't fully supported

## Drawbacks

-Compilation (Browsers don't understand typescript, so we have to give it to the ts compiler to compile it to js, this process is none as transpilation)

- We have to be a little bit more discipline when using ts

**Typescript is perfect for both small and big project where as javascript is perfect for small project and not big projects**

## `Npm i -g typescript` to installtypescript compiler

## `tsc -v` to check it's version on your machine

After modifying our ts file, we run `tsc index.ts` (using index.ts as an example) to compile it to index.js

Use `tsc --init` to generate a tsconfig.json file

## Typescript Types

-Any: the any type basically makes our code behaves like javascript , where we can set a variable to a name, then change it to a string or whatever, this should be used with caution.
(`let number: any = 90`)

- Array : When working with arrays in js, the values of the array can be dynamic e.g `let arr = [1,2,"3"]` but what if we want an array of just numbers? Then we use `let arr : number[] = [1,2,"3"]` at this point, ts will thrrow an error for the last value

-Tuple: We use tuple when we want to set a fixed array length and type for each element in the array.
(`let user: [number, string] = [1, "Raj", 0]`) this will throw an error because we were expecting just 2 elements with the first been a number and the second been a string

- A good length for tuples is 2, anything more than two and your code start looking weird

**Gotchas:** Even tho we set a tuple to two, the array push method can be used to add more elements.
