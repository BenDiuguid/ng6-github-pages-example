# ng6-github-pages-example

After a fresh `ng6 new app:web <app-name>` and pushing your project to a repo on GitHub, one can simply run one of the following commands.

```shell
yarn add -D gh-pages
```

or

```shell
npm install --save-dev gh-pages
```

Then add the following 2 lines to you're `package.json`'s scripts entry

```json
"predeploy": "npm run build",
"deploy": "gh-pages -d build",
```

Then execute `npm run deploy` to deploy your web app to `https://<github-username>.github.io/<repo-name>`
