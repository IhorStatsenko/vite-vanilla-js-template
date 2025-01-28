### gh-pages setup

1. create repository
2. open in gh desctop
3. npm create vite@latest
4. npm i
5. npm run dev
6. ? git config --local core.autocrlf false
7. create vite.config.js

```
import { defineConfig } from 'vite';

export default defineConfig({
  base: '/<repository-name>',
});
```

8. in package.json add the following

```
...
"homepage": "https://<your-username>.github.io/<repository-name>/",
...
"scripts": {
    ...
    "predeploy": " npm run build",
    "deploy": "gh-pages -d dist"
  },
  ...
```

9. npm install gh-pages
10. git .add + commit to save changes
11. npm run deploy

12. use https://<your-username>.github.io/<repository-name>/

### add-test-scss

1. npm add -D sass
2. npm install normalize.css
