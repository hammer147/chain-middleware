# Chaining Middleware

Next.js will look for a middleware.ts file (at the same level as the app folder) that exports a function, usually called middleware.

If we have a lot of middleware to handle (auth, error handling, setting headers, logging, ...) it would be messy to have it all in one function.

In those cases, we can separate them in higher-order functions in different files and combine them using a recursive chain function that we export in our middleware.ts file.

This concept is well explained in this [blog post](https://reacthustle.com/blog/how-to-chain-multiple-middleware-functions-in-nextjs)
