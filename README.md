# Vue 3 + TypeScript + Vite + eslint + prettier +commitlint + styleLint + standard + husky + lint-staged

该项目为 前端快递开发模版 做了各类语法检查、以及在主分支的推送和 pr 时，对进行 ci 检测(是否项目能正常 build、
以及 eslint 是否通过)

## 下载安装

使用 fork 或者 使用[degit](https://github.com/Rich-Harris/degit)
`npx degit Eveimo/fast-start-vite#main my-project` `cd my-project` `npm install` `npm run dev`

## 使用

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with
`vue-tsc` for type checking. In editors, we need
[TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)
to make the TypeScript language service aware of `.vue` types.

If the standalone TypeScript plugin doesn't feel fast enough to you, Volar has also implemented a
[Take Over Mode](https://github.com/johnsoncodehk/volar/discussions/471#discussioncomment-1361669) that is
more performant. You can enable it by the following steps:

1. Disable the built-in TypeScript Extension
   1. Run `Extensions: Show Built-in Extensions` from VSCode's command palette
   2. Find `TypeScript and JavaScript Language Features`, right click and select `Disable (Workspace)`
2. Reload the VSCode window by running `Developer: Reload Window` from the command palette.
