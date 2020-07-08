# share-snippets-demo

VS Code插件[Share Snippets](https://marketplace.visualstudio.com/items?itemName=sugar.snippet&ssr=false#overview) 支持的代码片段示例npm package

>VS Code Plugin [Share Snippets](https://marketplace.visualstudio.com/items?itemName=sugar.snippet&ssr=false#overview) Support code snippets demo npm package

## 目录 category
```bash
.
├── README.md
├── package.json
├── share_snippets
│   ├── comment                     # 注释相关
│   │   └── comment.code-snippets
│   ├── components                  # 组件相关
│   │   ├── comonent.code-snippets
│   │   └── myButton.share-snippets
│   ├── js                          # js相关
│   │   └── js.code-snippets
│   └── vue                         # vue相关
│       └── vue.code-snippets
├── test                            # 测试自定义片段的文件
│   └── test.vue
└── transferFileToSnippetBody.js    # 功能函数
```
## Snippets规则,如何编写
> Snippets rules, how to write
* [简体中文](https://juejin.im/post/5d0496415188257fff23b077#heading-3)｜[English](https://code.visualstudio.com/docs/editor/userdefinedsnippets#_create-your-own-snippets)

## 本仓库中的 Snippets
>Snippets in this project

`share_snippets`目录中的内容

| prefix |             scope              |          comment           |
| :----: | :----------------------------: | :------------------------: |
| author |   javascript,typescript,vue    |        author info         |
|  ctdl  | javascript,typescript,vue，jsx |     TODO Comment Line      |
|  ctdb  | javascript,typescript,vue，jsx |     TODO Comment Block     |
| vcapi  | javascript,typescript,vue，jsx | Vue Component-api template |
|  ctdb  |              vue               |         Array Fill         |

## 如何快速生成snippet中的body的内容
>How quickly generate the content of body in snippet

`TIPS：需要安装Node`

>`TIPS: Need install Node`


使用提供的`transferFileToSnippetBody.js`文件

>Use the provided `transferFileToSnippetBody.js` file
```js
node transferFileToSnippetBody.js filename1 filename2 filename3 ...
```

快速将指定的文件中的内容转成 `[context]`的形式
>Quickly convert the contents of the specified file into the form of `[context]`
demo：
```js
node transferFileToSnippetBody.js test.vue
```
会在当前目录下生成`test.vue.json`文件里面的内容即可直接粘贴到`.code-snippets`文件的`body`属性中

>The content in the `test.vue.json` file generated in the current directory can be directly pasted into the `body` attribute of the `.code-snippets` file