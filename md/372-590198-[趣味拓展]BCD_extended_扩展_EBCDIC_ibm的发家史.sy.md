---
show: step
version: 1.0
enable_checker: true
---

# 编码进化

## 回忆上次内容

- 上次 回顾了
	- 数字 进入二进制世界的 过程
- 采用的编码 是 BCD
	- `B`inary `C`oded `D`ecimal
		- 也叫8421码
		- 十进制数的 二进制形态
- 数字的 输出形式
	- 辉光管
	- 七段数码管
		-	7-seg 

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667295109705)

- 除了数字 之外
	- 还有 字母
- 字母 是如何编码进入 计算机世界的 呢？🤔

### BCDIC

- 在BCD的 基础上
	- ibm 继续着 人口统计的工作
	- 除了数字之外
	- 有了 字母编码的需求

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20210226-1614322193147)

- ibm制作了一种 6-bit 的字符编码格式
  - BCDIC
	- Binary Coded Decimal Interchange Code
  - 是一种 6-bit 的编码
  - 是一种 以纸带为核心的 编码
- 在BCD的基础上 添加了字母
	- 字母 按照十进数 编码
- 为什么 不按 二进制数 编码呢？🤔

### 输入

- 输入的设备 是 数字键盘		
	- 3个十进制数字输入1个字母

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667290576172)

- 数字键盘 在固定电话中 依然存在

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20230209-1675952131836)

- 有点像 九键输入法
- 当时的 ibm 
	- 是 数字世界的 领航员

### ibm

- ibm从一开始
	- 玩的 就是数字化
	- 以人口统计 起家

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667299899273)

- 到 称重计价

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667299930617)

- 再到 上班打卡

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667299948164)

- 数字化 根本离不开ibm
	- ibm开始逐渐盲目自大
	- 酝酿了隐患

### 隐患

-  数字键盘
	- 符号部分需要四次按键

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667290576172)

- BCDID
	- 本来连续的 6-bit 当中
	- `4` 行 `12` 列 本应连续

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667299681208)

- 红色部分造成
	- 字母序号 不连续
- 这 是个 小小的隐患

### 行列

- BCD扩展后的 BCDIC

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20210226-1614322193147)

- 6 位 2进制数字
	- 可以记录 1个字符

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20211001-1633043601703)

- 6-bit的编码

### 继续发展

- ibm业务 越来越多
	- 各国都要统计数据

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667300507678)

- 业务 越来越多
	- 编码方式 大同小异
	- 但是 随着业务的不同
	- 每次的编码 也有 调整

### 商业 公司

- 商业公司 也想要 统计数据
	- ibm也接下

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667300581407)

- 业务多了
	- BCDIC 这个编码本身
		- 也在随着业务的增多不断发展变化

### 问题

- ibm 在数字化的过程中 机会很多
	- 随着业务的`变化` 
		- BCDIC编码 也跟着 `变化` 
	- 造成了 编码本身的 不稳定

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20210226-1614322351627)

- 后面的代码
	- 并不能 和前面兼容
	- 那个时候 还没有向下兼容的 概念

### 后来

- 混乱之上的混乱就显得更加混乱🤪
  - 总共有 6 个不兼容的编码🤪
  - 每个编码都不同🤪
  - 各个编码之间不能相互转化🤪
  - 甲方不得不花钱来进行转化？🤫

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221021-1666357620295)

- 话说编码不应该是最开始就想好么？
  - 现实却是设计跟着思路
  - 思路跟着需求走
- ibm 终于意识到不同的格式之间应该编码统一了 😓

### 编码细节

- 由于 编码不兼容
	- 导致 旧的数据不能用了
- 这个编码转化 `没`人知道怎么弄
  - 成了 IBM 历史上 最大黑点和最高机密
- 那是一段 
	- 从继电器 IBM704
	- 到晶体管 IBM1401
	- 再到集成电路 
	- 再到cpu的历史
- IBM今天
  - 仍然是银行和金融系统 `最`相信的系统集成商
	  - 历史上游的优势
		- 真的很厉害

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20210226-1614324059760)

- 后期编码中 
	- 基本数字和字符 
		- 比较稳定
	- IBM 也有了 专门 进行解码的打印机
- 但是 符号部分
	- 没有 统一的规范
	- 随着 业务变化
	- 处于 一个混乱的状态 中
- 为了兼容而兼容
	- 把隐患就给兼容进来了
- 为什么 要 这样编码 呢？

### 利于转化

- ibm 终于开始注意 向后兼容的问题
  - 这种新编码是要和原来的 6-bit 的编码兼容
  - 可以快速的转化

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221021-1666350464533)

- 按理说以 ibm 当时垄断的情况
  - 已经把这个编码做成自己的标准
  - 也就成了行业的标准
	  - RCA 和富士也开始以此标准制作兼容系统
		 - 兼容这种编码
- 在隐患上建立起再高的大楼
	- 也是要倒塌的

- 可是用什么编码来统一的呢？🤔

### EBCDIC

- ibm终于决心把字符编码定下来
	- 在BCDIC的基础之上 
	- 确立EBCDIC
		- Extended Binary Coded Decimal Interchange Code
		- [eb'si:dik]
	- 用一个字节来编码
		- 配合最新发布的8-bit计算机IBM360
	- 符号数量提升
- 前面是控制字符
  - NUL
  - DEL
  - CR(还记得什么意思么？)
  - NL(还记得什么意思么？)
- 黑暗森林 开始 慢慢成型😄

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221101-1667300941274)

- 但是注意 这EBCDIC和ascii 还不一样
	- 黑暗森林后面 是 字母和数字
- 字母排布 仍然 兼容BCDIC
	- 字符编码 并不连续
	- i和j之间的序号 相差不止1

### 向后兼容

- 字母部分 确实是 向后兼容的

![图片描述](https://doc.shiyanlou.com/courses/uid1190679-20221021-1666350526261)

- 不过 这套排布方式
	- 和ascii 并不一致
- 虽说 这种编码 `有`缺陷
	- 但是 `已经`形成了 行业标准
- ascii究竟是 如何 从`无`到有
	- 能否打败 强大的蓝色巨人IBM
	- 在编码大战中 笑到最后 呢？

## 总结

- 这次 回顾了 字符编码的 进化过程
  - IBM 在数字化过程中
	- 作用  非常大
    - IBM 的 BCDIC 有 黑历史 😄
- 6-bit的 BCDIC 
	- 直接进化成 8-bit的 EBCDIC
	- 补全了 小写字母 和 控制字符
- 在ibm就是信息产业的年代
	- ibm的标准 怎么最终
		- 没有成为 行业的标准 呢？🤔
- 我们下次再说！👋