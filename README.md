# `wheel-factory`

> 简单、有趣的轮子工厂

## Development

使用本地的 lerna，而不是全局的 lerna

**安装全部依赖**

一般第一次拉到本地的时候使用

```
npx lerna bootstrap
```

**列出所有的包**

```
npx lerna list
```

**安装依赖**

lerna add <package>[@version] [--dev] [--exact]

> 增加本地或者远程package做为当前项目packages里面的依赖

- --dev devDependencies 替代 dependencies
- --exact 安装准确版本，就是安装的包版本前面不带^

**创建一个新包**

lerna create <name> [loc]

> 创建一个包，name包名，loc 位置可选

**导入依赖**

lerna import <path-to-external-repository>

> 导入本地已经存在的包

**执行脚本**

lerna run [--scope my-package] <script>
