# 重要命令
考虑使用icloud共享目录，命令的运行旨在只做必要改动，每本书的阅读都有自己的目录，所有书共享一个font目录
```sh
## 古文观止
cd ./gwgz
font assignment -book gwgz #批量生成作业，运行一次后很少要跑

#叠加方式编辑字体文件, 作业文件名可以通过tab辅助填写,font文件在不同的书籍阅读中积累，所以放到上一级目录
font typeface -font-name Kexin -handin ./handin/<指定作业文件名> 
#批量重新生成所有字的字体
font typeface -font-name Kexin -handin ./handin

#逐一添加的方式生成html, 课文文件名可以通过tab辅助填写
font publish html -font-name Kexin -text ./text/<指定课文文件名> 
# 可心每次handin过得课文被复制到./text/done，因此字库每次更新时也可以批量化重新生成html
font publish html -font-name Kexin -text ./text/done
# 可心每次handin过得课文被复制到./text/done，因此字库每次更新时也可以重新生成epub
font publish epub -font-name Kexin -text ./text/done -epub-name 古文观止-可心手抄本
```

```sh
## 东坡诗话
cd ./dpsh
font assignment -book dpsh -text ./text/20260908   #东坡诗话的数据源没有经过切割，以晶晶的阅读进度按日交给可心学习和写字
font typeface -font-name Kexin -handin ./handin/<指定作业文件名> #叠加方式编辑字体文件, 作业文件名可以通过tab辅助填写,font文件在不同的书籍阅读中积累，所以放到上一级目录
font publish html -font-name Kexin -text ./text/<指定课文文件名> #逐一添加的方式生成html, 课文文件名可以通过tab辅助填写
```

# 学习书目
- gwgz [古文观止](https://github.com/jeankueo/guwenguanzhi)
- dpsh [东坡诗话](https://github.com/jeankueo/poem/blob/master/%E8%AF%97%E8%AF%9D/%E4%B8%9C%E5%9D%A1%E8%AF%97%E8%AF%9D.txt)

# 参考链接
- [数据来源](https://github.com/niuniu-869/guwenguanzhi)
- [在线浏览](https://niuniu-869.github.io/guwenguanzhi/)

# 游戏时间兑换
## 积分榜
|课文编号|活动|字数|完成日期    |兑换日期和游戏时间        |
|---    |---|---|---         |---                    |
|001-p1 |抄写|   |before     |/                      |
|001-p2 |抄写|   |before     |           - 5行兑换1下午|
|001-p3 |抄写|   |before     |2026.09.15 - 3行兑换1小时|
|001    |阅读|   |before     |/                      |
|008    |抄写|36 |2026.09.14 |2026.09.14 - 3行兑换1小时|
|016    |抄写|   |before     |/                       |
|018    |抄写|   |before     |/                       |
|027    |抄写|   |before     |/                       |
|039    |抄写|   |before     |/                       |
|040    |抄写|   |before     |/                       |
|047    |抄写|12 |2026.09.14 |                    - 1行|