# Markdown 学习笔记

记一些排版的注意点和一些好玩的小技巧

记录语法没有意义



## 0.目录

[TOC]

 

## 1.排版

自己喜欢的风格, 没有任何的普适性

唯一的原则是风格的统一

### 1.3 标题

详情可见目录

只使用一级标题到四级标题

一级标题是自己文档的题目, 一个文档允许有一个一级标题

二级标题, 数字加点无空格, 如: `1.第一个二级标题` , `01.第一个二级标题` ; 是 `1` , 还是 `01` 风格统一就好

三级标题, 二级标题逗号加数字再空格, 如: `1.1 三级标题` , `01.1 三级标题` 

四级标题, 三级标题短横线加数字再空格, 如: `1.1-3 四级标题`

五级标题六级标题不建议使用, 建议用无序的代替, 其字体大小已经和加粗很很难区分

### 1.2 空格

- 统一使用英文标点, 标点前不空格, 标点后必须要一个空格, 每一行结尾的句号, 可加可不加, 但在一个文档的内部, 格式要统一
- z左括号前要有空格, 后面不要有空格, 除非是代码块; 有括号对称, 如: 我 (任家平) 是; 我 ( `rjp` ) 不服 
- 链接, 锚点, 单行代码块... 前后都需要空格, 为了避免在其结尾一行时, 光标移动至其后方自动弹出链接; 多个单行代码块并列, 如: `123` , `234` , `46` 
- `sfdas` : 前面有空格, 后面也有空格
- 英文中文切换处需要空格, 如: 我名字缩写是 rjp, 它是我名字的缩写; 如果这样 USB2.0 是无法使用的; 但如果只有一个英文字母 g, 像这样, 后面直接跟着标点, 那么左边有空格, 右边直接跟标点

### 1.3 空行

- 目录一般在一级标题与第一个二级标题之间, 其上下各空一行; 若没有目录, 则一级标题和第一个二级标题空一行

- 二级标题的结尾与下一个二级标题要空一行; 低级别标题之间不用空行



## 2.好玩的东西

- flow流程图的使用

```flow
st=>start: 开始
op=>operation: My Operation
cond=>condition: Yes or No?
e=>end
st->op->cond
cond(yes)->e
cond(no)->op
```

```flow
st=>start: index
op=>operation: 申请
op2=>operation: 结果页
op3=>operation: 查询本地
i1=>inputoutput: bid入库
i2=>inputoutput: 填写个人信息
c1=>condition: 检查登录
c2=>condition: 登录
c3=>condition: 查询本地记录
c4=>condition: 检测状态
c5=>operation: 风控审核
e=>end

st->op->c1()
c1(no)->c2(yes)->op()
c1(yes)->c3(no)->i1(right)->i2(right)->c5()->op2->e
c1(yes)->c3(yes)->c4(no)->i2
c1(yes)->c3(yes)->c4(yes)->op3->op2
c3()->e
```



- checkbox的使用

- [x] fdsfa
- [ ] fsdfas

- 表格

  | 学号 | 学生 |
  | ---- | ---- |
  |      |      |


- 锚点的使用

  只能链接到标题, 适合自己做目录, 但我一般用toc语句

  [01](#rrr)

  jflsd
  d
  fds
  fd

  sdf
  dsf
  ds
  fds
  fds
  fds
  f
  dsf
  dsf

  ### rrr
