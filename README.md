多云基础设施编排工具Terraform,重点解决公有云厂商的软硬件（基础）资源构建的问题。 公司最近用上了terraform, 新建服务, 更改配置, 增加SG都要通过它进行.

terraform是个什么东西呢? 想一下, 其实就是在各个云平台提供的API之上, 搞出来一个抽象层.

Terraform的生态环境到了今天，已经发展为三个分支，分别是：
1）开源版
2）Terraform Cloud云服务版
3）Terraform企业版

更多资料参考： 
http://registry.terraform.io/browse/providers 


https://lonegunmanb.github.io/introduction-terraform/


![图片](https://user-images.githubusercontent.com/2436384/158143039-bbb632d5-7301-46e1-9590-ed6e5c7da266.png)

![图片](https://user-images.githubusercontent.com/2436384/158143092-914a6cd4-faf6-4201-9f93-9d1ecb4888d7.png)

![图片](https://user-images.githubusercontent.com/2436384/158143118-3b904a95-469a-41fe-9fc2-3597e07861df.png)



> 《Terraform 101 从入门到实践》这本书只将在[南瓜慢说官方网站](https://www.pkslow.com/tags/terraform101)和[GitHub](https://github.com/LarryDpk/terraform-101)两个地方同步更新，如果你在其它地方看到，那应该就是抄袭和未授权的转载。书中的示例代码也是放在GitHub上，方便大家参考查看。

---

# Terraform 101 从入门到实践
Terraform作为基础设施即代码（Infrastructure as Code，很简称IaC）的事实标准，非常值得大家学习。我是工作中会使用公有云，所以需要经常使用Terraform作为IaC工具以实现自动化部署；也花时间考取了**Terraform Associate**的证书。所以对它的使用我还是有一些经验的。但Terraform本身发展是比较快的，国内的资料也相对较少，所以我整理了我的学习心得，希望可以帮助到大家。

因此，我做了一个决定，将知识点整理成书，叫《Terraform 101 从入门到实践》。我之前在我的博客也写了[Terraform系列的文章](https://www.pkslow.com/tags/terraform)，还相对还是比较零散，不够系统和全面，所以还是决定尝试写书吧。

该书会不断增加和完善内容，所以初期会有很多不完美的地方。如果大家有问题可以提Issue，但前期不会处理。~~我的目标是在2022年5月11日前完成，希望不要鸽~~。因为工作变动原因，我需要学习和适应，没有ETA，慢慢更新吧。

目前进度可能大概是42%？我也不确定。哈哈，佛系更新。但Terraform的基本概念是已经介绍了的，了解与入门是够用了。代码目前没有整理上传，但在文章中都会有，不影响大家理解。我会尽量在工作之余、带娃之余、睡觉之余挤时间完成。这篇文章也算是立个Flag，并自我监督吧。


进度条：
<div style="width: 100%;background-color: #ddd;">
<div style="width: 42%; background-color: #5d21d0;
text-align: right;padding-right: 20px;
line-height: 40px;color: white;">
  42%
</div>
</div>






如果大家觉得不错，可以好心给个STAR支持一下哦。你的鼓励，是我的动力。


**博客目录**：

- [前言](https://www.pkslow.com/archives/terraform-101-preface)
- [第一章 Terraform初相识](https://www.pkslow.com/archives/terraform-101-introduction)
- [第二章 Providers插件管理](https://www.pkslow.com/archives/terraform-101-providers)
- [第三章 Modules模块化](https://www.pkslow.com/archives/terraform-101-modules)
- [第四章 States状态管理](https://www.pkslow.com/archives/terraform-101-states)
- [第五章 HCL语法](https://www.pkslow.com/archives/terraform-101-hcl)
- [Functions函数](https://www.pkslow.com/archives/terraform-101-functions)
- [Terraform常用命令](https://www.pkslow.com/archives/terraform-101-commands)



**GitHub目录**：

- [前言](https://github.com/LarryDpk/terraform-101/blob/main/README.md)
- [第一章 Terraform初相识](https://github.com/LarryDpk/terraform-101/blob/main/01.Terraform初相识.md)
- [第二章 Providers插件管理](https://github.com/LarryDpk/terraform-101/blob/main/02.Providers插件管理.md)
- [第三章 Modules模块化](https://github.com/LarryDpk/terraform-101/blob/main/03.Modules模块化.md)
- [第四章 States状态管理](https://github.com/LarryDpk/terraform-101/blob/main/04.States状态管理.md)
- [第五章 HCL语法](https://github.com/LarryDpk/terraform-101/blob/main/05.HCL语法.md)
- [Functions函数](https://github.com/LarryDpk/terraform-101/blob/main/Functions函数.md)
- [Terraform常用命令](https://github.com/LarryDpk/terraform-101/blob/main/Terraform常用命令.md)
- Terraform在公有云的应用（未开始）
- Terraform问题定位与分析（未开始）
- 插件开发（未开始）
- 最佳实践（未开始）
- 开发套件（未开始）

---






最后，附上我的Terraform证书：

<img src="https://pkslow.oss-cn-shenzhen.aliyuncs.com/images/other/terraform-101/pictures/00.preface/terraform-associate.certificate.png" width="300">



<img src="https://pkslow.oss-cn-shenzhen.aliyuncs.com/images/other/terraform-101/pictures/00.preface/terraform-associate.certificate-larry.png" width="300">



