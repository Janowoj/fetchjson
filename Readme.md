This is a small app, which goal is to show how to use Typescript to fix some of the bugs.

To execute this file we have to compile it first. To do so, we have to run the following command:

`tsc index.ts`

I creates a new file called index.js, which is the compiled version of the index.ts file.

Now we can run the file with the following command:

`node index.js`

We can combine both commands in one with the following command:

`ts-node index.ts`

# How to fix the bugs

When we mess with the properties of an object, we can get some errors. To fix them, we have to define the type of the object.

We didn't know the bug existed until we actually executed the file.

````interface Todo {
  id: number;
  title: string;
  completed: boolean;
} ```

```const todo = response.data as Todo;```
````

Now Typescript knows that the object todo has the properties id, title and completed.
It underlines the properties that we are not using, so we can delete them.
