---
layout: post
title: "node path"
date: 2017-09-24 12:15:06 
description: "node file path,always forget,so write down"
tag: node
---


- 相对路径之当前目录：./xxx/xxx.js 或 ./xxx/xxx。
- 相对路径之上级目录：../xxx/xxx.js 或 ../xxx/xxx。
- 绝对路径：F:/xxx/xxx.js 或 /xxx/xxx.js 或 /xxx/xxx。


![image]( Lock-And-Key.github.io/images/posts/Node-Path/07131745-f8df335fb6d2424cbaf997109a647dcd.jpg )


```
1 require('module_1_1.js');
2 require('module_1_2');
3 require('../node_modules/module_2_1.js');
4 require('../node_modules/module_2_2');
5 require('../package_2_1');
6 require('package_3_1');
7 require('./node_modules/package_3_2');
8 require('module_3_1');
9 require('/node_study/level1/level2/level3/node_modules/module_3_1');
10 require('module_3_2');
11 require('/node_study/level1/level2/level3/package_3_3');
12 require('./package_3_4');
13 require('./module_3_3');
14 require('same_name_module');
15 require('same_name_package');
16 require('same_name_module_and_package');
```

```
1 module_1_1.js
2 module_1_2.js
3 module_2_1.js
4 module_2_2.js
5 package_2_1
6 package_3_1
7 package_3_2
8 module_3_1.js
9 module_3_2.js
10 package_3_3
11 package_3_4
12 module_3_3.js
13 same_name_module.js in leaf
14 same_name_package in leaf
15 same_name_module_and_package.js in leaf module
```
