---
title: markdown语法扫盲
date: 2019-02-23 15:10:06
tags:
    - markdown
---

## 粗体,`**，__`
> ` **粗体**`
> **粗体**

## 斜体,`*,_`
> `*斜体*`
> *斜体*


## 标题 `#`
  # `#`一级标题
  ## `##` 二级级标题
  ### `###` 三级级标题
  #### `####` 四级级标题
  ##### `#####` 五级级标题
  ###### `######` 六级级标题

   > 一级标题
   > `==`
   > 二级标题
   > `--`

多于一个`=`,`-` 分别代表一级标题，二级标题

## 插入链接

`[文本](url,textalt)`
[百度](http://www.baidu.com "百度")

## 插入图片
`![图片描述](url)`
![qqlogo](https://mat1.gtimg.com/pingjs/ext2020/qqindex2018/dist/img/qq_logo_2x.png)

## 无序列表
`+,-,*`
- 无序列表
- 无序列表
- 无序列表

## 有序列表

使用非负数字+ `.` ,非负数不一定从1递增
当有序列表的第一行是0.时从0开始递增，多级列表的第二级开始不支持从0开始

```
1. 这是一级有序列表
    1. 这是二级有序列表
    1. 这是二级有充列表
        1. 这是三级有序列表
8. 这是一级有序列表
0. 这是一级有序列表
```
1. 这是一级有序列表
    1. 这是二级有序列表
    1. 这是二级有充列表
        1. 这是三级有序列表
8. 这是一级有序列表
0. 这是一级有序列表

## 引用

`> 这是引用`
> 这是引用

## 代码块

被\`\`\`包围的段落称为代码块(有些Markdown解释器支持语法高亮)


## 分隔符行

三个或者多于三个 -,+,_；不能有其它内容，单独在一行

`----`
 ----
`****`
 ****

## 表格

Markdown之父 John Gruber 和 Aaron Swartz 发布的Markdown解释器中没有表格格式，目前一般使用的表格格式是GFM的扩展

```
表格字段一|表格字段二|表格字段三|表格字段四
--|:--|--:|:--:
默认居中对齐|左对齐|右对齐|居中对齐
cell|cell|cell|cell
```
表格字段一|表格字段二|表格字段三|表格字段四
--|:--|--:|:--:
默认居中对齐|左对齐|右对齐|居中对齐
cell|cell|cell|cell
