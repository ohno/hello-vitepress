# Hello VitePress

1. Add [Node.gitignore](https://github.com/github/gitignore/blob/main/Node.gitignore).
2. Select [VitePress theme](https://www.builtatlightspeed.com/category/vitepress).
3. Install and start [VitePress](https://vitepress.dev/guide/getting-started):
    1. `npm add -D vitepress@1.6.3`,
    2. `npx vitepress init`,†
    3. `npm run docs:dev`.
4. Visit ［`https://github.com/user/repo-name/settings/pages`](https://github.com/ohno/hello-vitepress/settings/pages) and set "Source" to "GitHub Actions".
5. Add `base: '/repo-name/', ` to `.vitepress/config.mts`. https://github.com/ohno/hello-vitepress/blob/d91abf9b46e713128c95a2ad204ed5d2e03a14d7/.vitepress/config.mts#L5
6. Add [deploy.yml](https://vitepress.dev/guide/deploy#github-pages) and change `path: docs/.vitepress/dist` to `path: .vitepress/dist` for GitHub Pages. https://github.com/ohno/hello-vitepress/blob/e13e2915118641d1796544626c1796ee119e24f8/.github/workflows/deploy.yml#L53  

†
```sh:
> npm add -D vitepress@1.6.3

> npx vitepress init        

┌  Welcome to VitePress!
│
◇  Where should VitePress initialize the config?
│  ./
│
◇  Site title:
│  My Awesome Project
│
◇  Site description:
│  A VitePress Site
│
◇  Theme:
│  Default Theme
│
◇  Use TypeScript for config and theme files?
│  Yes
│
◇  Add VitePress npm scripts to package.json?
│  Yes
│
└  Done! Now run npm run docs:dev and start writing.

> npm run docs:dev
```
