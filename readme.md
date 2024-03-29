### 原由
近期需要对一些域名来进行一些特殊的处理．例如提取域名的主域名．
```
www.baidu.com => baidu.com
ai.baidu.com => baidu.com
```
提取域名时就需要对已有的域名后缀来进行对应的匹配．但是已有的域名后缀没有一个完整的库．查询了很多都没有．所以就有了一个这样的想法．以社区的力量来整合这个域名后缀，同时也方便域名抢注或域名注册商接入这些新的域名后缀．在域名中，其中，大概分为两类，一类是通用顶级域名(GTLD)，一类是区域性或地区性的二级域名(CCTLD). 同时这个仓库还会收集对应域名的whois服务器. 方便后面对接所有的whois. 也可以让自己成为一个域名抢注商(黄牛). 提高大家的域名版权概念.
### 通用顶级域名(GTLD)
顶级域名, 大部分由iccan来维护，当然有的顶级的域名后缀是由其他的组织来进行维护的．例如 .cn. 这里我们只统计顶级域名.
### 地区性域名(CCTLD)
地区性域名泛指由国家和地区来进行维护的域名．例如.cn. 这类下面就会有很多的二级子域. 例如. .政务.cn, .hb.cn等等. 这里也是我们需要收集的.
### 如何贡献
如果有需要补充的请提交Pull Request来进行提交．提交时，请提供对应地区性域名或顶级域名的管理者．例如
```
.aaa|American Automobile Association, Inc.
```
如果是提交地区性域名，请提供对应的readme和公布信息．如下
```
.cn [中国域名互联网体系](http://xn--eqrt2g.xn--vuq861b/)
```
并以地区或国际的英文代码来进行命名，详细参考 cctld/china 这个文件夹
### 目录结构说明
```
├── cctld   // 地区性域名
├── data    // 未整理的原始数据
├── gtld    // 顶级域名
└── readme.md
```