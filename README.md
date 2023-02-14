# Webpack基础，进阶，高级

- webpack基础：包含是什么，有什么用，如何使用。
- webpack高级：Webpack高级优化配置，提升项目打包和运行时性能。
- webpack项目：从零开始搭建一个项目脚手架，并进行优化（包含React和Vue）
- webpack原理：Webpack Loader和Plugin原理。

## Webpack
webpack是一个静态资源打包工具
它会以一个或多个文件作为打包的入口，将我们整个项目所有文件编译组合成一个或多个文件输出出去。
输出的文件就是编译好的文件，就可以在浏览器端运行了
我们将Webpack输出的文件叫做bundle。

webpack就是将浏览器不能识别的语言（如ts，less，sacc）等编译成浏览器可以识别的代码，这个过程叫做打包。

- webpack本身功能是有限的
    - 开发模式：仅仅能够编译js中的ES Module语法
    - 生产模式：能够编译js中的ES Module元，还能压缩js代码

## npx的作用
- npx webpack：npx的作用是将node_modules中的./bin目录临时添加为环境变量。
- npx webpack ./src/main.js --mode=development  开发环境
- npx webpack ./src/main.js --mode=pdoduction   生产环境