+++
draft = true
author = "Rumn"
title = "readme"
date = "2026-09-28"
description = "写给自己的说明书"
weight = 0
+++

==2026/10/01 新增数学公式渲染==
	在front matter加入 "math = true"即可开启数学公式渲染（不默认开启是防止速度太慢）

==2026/09/30 文档内部跳转==
文档内部也可以实现跳转，多级小标题每个都是一个锚点
\[跳转名\](\#标题名)  就可以了，不要漏掉井号

==2026/09/30 本地文件夹嵌套==
由于设置了逐层挖掘，可以嵌套多级文件夹方便本地管理（但注意各种文件夹的分类作用只在本地有效）。

==2026/09/30 series==
关于series：
	1、翻页是按照weight来定的，并且weight排序只在series内有效（其他都是按日期）
	2、必须加一下front matter，尽量一个都不要少
	
			+++
			
			author = "Rumn"
			title = "..."
			date = "xxxx-xx-xx"
			description = "..."
			
			tags = [
			    "..."
			]
			categories = [
			    "...",
			]
			series = [
				"..."
			]
			
			weight=...
			
			+++
			
注意日期格式，错了会解析不出来。

==2026/09/29 文件名和路径==
渲染后的路径名就是obsidian里的文件名，而title那个是网页上显示的名字。
所有路径一定小写（不然github会解析错误）
而title就可以加中文和emoji
