# How to replicate issue #4332

After cloning the repository please perform the next steps.

1. cd into `dummy-linked-module` and run `yarn link`.
2. cd into `project` and run `yarn link dummy-linked-module`.
3. run `yarn` to install Parcel 2.
4. run `yarn dev` in order to start the dev server.
5. open `dummy-linked-module/index.js` and change the console log message.

You will see that the message didn't change in the dev server because Parcel didn't rebuild.
If you are not familiar with `link` functionality of NPM/Yarn then please read:
https://docs.npmjs.com/cli/link.html
and/or
https://yarnpkg.com/cli/link
