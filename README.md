### 简介：
> 这是我发布的第一个第三方库小demo，实现了简单的功能：
> 把1-5的数字转换成文本形式，也可以将英文的文本字符转换成1-5的数字
> 让我们一起学习造轮子吧。

### 此插件需要依赖lodash
### 请确保你的项目中已经安装了lodash
#### 安装方式：
##### * npm的安装方式：
1. 执行 npm i dxm-numbers，如果发生以下错误的话请执行第二步
```
npm ERR! code ERESOLVE
npm ERR! ERESOLVE unable to resolve dependency tree
npm ERR!
npm ERR! While resolving: webpack_confusion@1.0.0
npm ERR! Found: webpack@5.75.0
npm ERR! node_modules/webpack
npm ERR!   dev webpack@"^5.75.0" from the root project
npm ERR!
npm ERR! Could not resolve dependency:
npm ERR! peer webpack@"^4.0.0" from uglifyjs-webpack-plugin@2.2.0
npm ERR! node_modules/uglifyjs-webpack-plugin
npm ERR!   uglifyjs-webpack-plugin@"^2.2.0" from the root project
npm ERR!
npm ERR! Fix the upstream dependency conflict, or retry
npm ERR! this command with --force, or --legacy-peer-deps
npm ERR! to accept an incorrect (and potentially broken) dependency resolution.
npm ERR!

npm ERR! A complete log of this run can be found in:
npm ERR!     D:\software\nodejs\node_cache\_logs\2023-01-11T11_27_42_026Z-debug-0.log
```
2. 执行 npm i dxm-numbers --legacy-peer-deps
3. 在页面中使用

```
import {numToWord,wordToNum} from 'dxm-numbers';
let res =  wordToNum('Five');
let res2 =  numToWord(1);

```
##### * script标签的方式引用
```
  <script src="/path/lodash.js"></script>
  <script src="/path/webpack-numbers.js"></script>
    let res =  myNumbers.wordToNum('Five');
    let res2 = window.myNumbers.wordToNum('Five');
```
