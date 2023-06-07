# 开始
> Crud Boy - Never get into ICU!

虽然这一段基本不太会有人看，但我还是得说如你所见，这只是另外一个快速开发的脚手架（[破轮子](about/broken-wheel.md)）而已，`如果你现在有着更好的选择，别用它`；

## 未曾开始先劝退
!> 当然我知道很多还在用 JDK8 的朋友很难理解，但目前后端采用 [Spring Boot 3.x](https://docs.spring.io/spring-boot/docs/current/reference/html/) 版本（不会回到2.x时代了），直接上 JDK 17+ 吧（也不知道咋想的，包名为啥要改，还 jakarta 我...）；

!> 后端用的是 JPA - 没有 Mybatis Plus，大佬们可能不太适应；

!> 前端现在只有一个 [Arco Design Pro - vue](https://arco.design/vue/docs/pro/start) 的实现，没有用 ElementUI 确实是看够了（而且不好看），没有用 Antd 确实是有点不习惯（膈应），没有用 React 确实是写不惯tsx（不会）（其实很想做ExtJS 7.x的，还是算了，要不然这破轮子更没人用）；

!> 这个破轮子并不太适合分工合作，适合前后端全部一把梭，省一个人的钱

## Features: 我不太会吹
- 代码生成器 - 注意这并不是一个低代码或者无代码平台（虽然CRUD确实不需要写代码），都是用 FreeMarker 生成的，前端的接口定义用 [@umijs/openapi](https://www.npmjs.com/package/@umijs/openapi) 通过后端的 openapi 来生成
- 基本不用操心数据库 - 因为用的是 JPA 而不是 MyBatis Plus 那种反向的生成，一切都是 Java ，当然是可以手写 SQL 的（但是要注意 JPA 同步数据库结构的弊端）
- 针对 JPA N+1 问题有不用写很多额外代码的解决方案，而且别听他们的，数据库的特性该用还得用
- 为了方便前后端一把梭而造的 [Schema](schema)，前后端统一用一套
- 为了方便前后端一把梭而做的统一多语言，虽然大部分情况用不上
- 代码质量还凑合 不能说多优雅多干净，说句不太脏应该还比较合适，尤其前端（因为有 eslint ...）我会尽量少写 any 的

> To be continued...