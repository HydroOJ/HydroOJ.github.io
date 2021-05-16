---
title: 感性理解 Hydro Online Judge 评测机综合水平
date: 2021-03-19
---
## 评测机配置

|     #      |              CPU              |     主频      | 评测机部署方式 |      评测机数量      |
| :--------: | :---------------------------: | :-----------: | :------------: | :------------------: |
|    UOJ     |  Intel Xeon Platinum 8269CY   | 2.5GHz~3.2GHz |       -        |          1           |
| CodeForces |      Intel Core i3-8100       |    3.6GHz     |   PC（推测）   |          -           |
|   Luogu    | Intel Xeon Platinum 8369HB/HC | 3.3GHz~3.8GHz |     阿里云     | $\infin$（弹性伸缩） |
|  HydroOJ   | Intel Xeon Platinum 8369HB/HC | 3.3GHz~3.8GHz |     阿里云     | $\infin$（弹性伸缩） |
|  LibreOJ   |       AMD Ryzen 5 3600X       | 3.8GHz~4.4GHz |       PC       |          1           |

由于 51nod 评测显示结果过少，无法获取其 CPU 信息。

---

## 评测速度

![](https://img-kysic-1258722770.file.myqcloud.com/fbecb593ca24c50eb7032a199bc9f683/b5fd6f6277693.png)

每项测试的源代码来自于 [感性理解 LibreOJ 测评机速度（2018 年 3 月 3 日之后）](https://loj.ac/article/425)。每项测试进行至少十次取平均运行时间（四舍五入）。时间以毫秒为单位。

由于 T5 在测试时需要超过 700MB 的空间，所以大部分 OJ 无法正常进行这项测试。

---

## 评测稳定性

![](https://img-kysic-1258722770.file.myqcloud.com/93111d07eef0fcbab4fc5336df59c0af/a404f4f8f30c1.png)

测试源代码与测试“评测速度”一块相同。取连续至少十次评测中最快用时和最慢用时之差。时间以毫秒为单位。

由于 CodeForces 不方便测试其稳定性，所以此处没有记录。

---

- [CodeForces](http://codeforces.com/) 测试时间 Apr. 10th 2018 （数据来自 [LibreOJ 的测试](https://loj.ac/d/425)）
- [Luogu](https://www.luogu.com.cn/) 测试时间 Mar. 3rd 2021
- [HydroOJ](https://hydro.org.cn/) 测试时间 Mar. 3rd 2021
- [LibreOJ](https://loj.ac/) 测试时间 Mar. 3rd 2021
- [UOJ](https://uoj.ac/) 测试时间 Apr. 22nd 2021
- [51nod](https://www.51nod.com) 测试时间 Mar. 4th 2021

由于近日 [Vijos](https://vijos.org/) 超过 99% 的评测任务已使用 [undefined](https://github.com/undefined-moe) 提供的使用 HydroJudge 进行评测的服务器进行评测，并不能代表其自身评测机速度，所以这里没有进行测试。

## 总结

Hydro Online Judge 采用了目前国内云服务器市场上能找到的运算能力最强的服务器为其提供评测服务，并采用弹性伸缩技术，理论上可以应对近乎无限并发量的评测任务。评测速度次于使用 PC CPU 的 LibreOJ，与 Luogu 相近。评测速度稳定性与 Luogu、UOJ 相近。总体上来说 Hydro Online Judge 在评测机方面上不逊于主流 OJ。
