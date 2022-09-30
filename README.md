VUE 源码分析
首先使用pnpm install 下载依赖
其次 将npm run dev 指令后面加上--sourcemap 如下： "dev": "rollup -w -c scripts/config.js --environment TARGET:full-dev --sourcemap"
根路径创建style文件夹，在各个html中进行调试 头部增加 <script src="../../vue/dist/vue.js"></script> 然后对应写vue代码即可
执行npm run dev 在 liveserver中打开对应html
修改源码 会自动重新打包 liveserver自动热加载