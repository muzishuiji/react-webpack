# react-webpack
一个从0-1的react项目,这里一步步实战react的常用特性,常用的优化策略,以及一步步配置webpack,以及webpack的一些优化实践.

由于项目中用到的特性受需求所限,所以对于react的很多特性我其实并不是非常熟知,所以想借助此项目把react的一些特性深入实战一下.

另外还有一个很重要的问题,就是工作中为了更快的启动和完成项目,会直接使用已经拥有完备配置的脚手架,所以导致对于webpack的打包配置优化知之甚少,
前几天看了一个webpack的系列教程和官方文档才知道,原来webpack还有这么多我不知道的妙用,所以也想借助这个项目自己动手从0-1去合理的配置一个项目,
并充分利用webpack提供的配置项对项目进行优化,同时自己动手实现一个loader和plugin,然后实现一个简易的boundler,以弥补开发过程中的经验确实和加
深自己对常用的技术的理解.该项目会包含的内容如下:

## react部分

1. 传统的class组件的编写,各个生命周期的使用

* shouldComponentUpdate: 对组件进行渲染优化
* 自定义事件的绑定:

自定义事件的绑定推荐使用在构造函数里使用bind的方式,而不推荐使用箭头函数等其他方式,这样会导致每次重新渲染都会创建一个新的函数,导致了性能的损耗和内存的浪费.

* pureComponent的使用



2. hooks组件的写法,hooks的各个api的使用

* useState
* useEffect

useEffect在使用的时候的优化注意点

* useCallback
useCallback在使用的时候的优化注意点

* useMemo

3. prop-types: 对传入的props做类型检查

4. render-props: 定义一个组件,可以自定义实现向vue中插槽一样的功能,后者接收一段逻辑代码,在组件的对应时机调用执行.

5. HOC: 高阶组件实战

6. 异步组件

## webpack部分

1. 常用的配置项的使用

2. splitChunks的使用
3. 关于sourcemap

4. tree shaking

5. 自定义loader

6. 自定义plugin

7. 打包公共代码

8. 第三方代码分开打包,提升打包速度

9. happypack

10. 打包性能分析

暂时就写到这里了,我会整理成一个博客分享,以分享的方式来促进自己的学习.
