# Google (Cloud Platform) Cloud Functions TypeScript starter project

This is a fork of the [original repository](https://github.com/amsokol/gcp-cloud-functions-typescript-starter) which contains a TypeScript starter for Google Cloud Functions.

I've added here some lacking and development dependencies and rewritten npm scripts to add some useful stuff.

You can start the function locally using [functions-framework](https://github.com/GoogleCloudPlatform/functions-framework-nodejs) with a single `npm run start` command.

In the same way as above, you can start the function locally in a watch mode using `npm run watch`. This command [concurrently](https://github.com/kimmobrunfeldt/concurrently) starts `tsc --watch` and [functions-framework](https://github.com/GoogleCloudPlatform/functions-framework-nodejs) with [npm-watch](https://github.com/M-Zuber/npm-watch). This way any modifications to the `index.ts` file are immediately visible after refreshing a browser. `tsc` currently generates map files for all generated `.js` so you can even use this feature to debug the function in a live mode. This can be done using running `npm run watch` in a debug mode from an IDE (WebStorm, Idea, etc).

Function can be deployed using `gcloud` command with `npm run deploy`.
