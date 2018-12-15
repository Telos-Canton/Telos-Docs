# 教你如何参与 Telos 节点投票（上）


大家好，Telos Canton 在这里为大家介绍投票操作，中间会穿插一些有用的小知识，也是大家经常会问及的。
我们会先介绍使用 Telos 官方钱包的投票方法，后面还会有Scatter钱包、Awake和欧柚手机端钱包的介绍。

### 第一步：下载官方松鼠钱包（Sqrl Wallet）
下载网址：https://github.com/Telos-Foundation/Sqrl/releases
Windows 用户选择“win-Sqrl-x.x.x.exe”
Mac 用户选择“mac-Sqrl-x.x.x.dmg”
Linux 用户……
下载完成安装软件。

### 第二步：导入EOS创世账户

当然，前提是你必须要有EOS创世帐户，步骤如下：

1. 选择“Telos Mainnet”，点击“Connet to Server”；

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_01.png)

2. 点击“Import Existing Account”；

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_02.png)

3. 输入你EOS创世账户的帐户名或公钥（注意是公钥而不是私钥），然后点击“Lookup Account”；

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_03.png)

4. 输入你的EOS创世帐户私钥，点击“Show private key”可以显示输入的字符，注意要在安全的环境下输入；

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_04.png)

5. 输入你的钱包密码，这是后面再登陆钱包和进行安全性操作时要用到的，请牢记；

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_05.png)

6. 最后，同意一些常规协议，你就可以对与EOS创世帐户等额（上限为4万个）的 TLOS 进行操作了！
![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_06.png)

### 第三步：投票
1. 点击钱包菜单栏的“Governance”，在“Block Producers”下面，点击选择30个BP，再点击“Submit votes for selected producers”进行投票；

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_08.png)

这里介绍一下为什么要选择30个，因为Telos取用“反向投票加权”（Inverse Vote Weighting）规则，这意味着如果你只投票给1或2个区块生产者，那么你的投票权重将低于投票给30个区块生产者的投票权重。目的是鼓励大多数Telos成员更多的去了解区块生产者候选人，并打击那些只为自己及其关系户投票的人。

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/inverse_weighted_voting_latex.jpg)
![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/inverse_weighted_voting.jpg)

你只要知道一点，如果投的节点数量少了，票力就会大打折扣的，所以，尽量投满30吧。

2. 点击“提交表决（Submit Votes）”完成投票。

![](https://raw.githubusercontent.com/Telos-Canton/Telos-Docs/master/images/howtovoteontelos/Telos_Sqrl_Voting_09.png)

是不是很简单？

补充一个小知识，Telos主网要在生产一百万个区块之后才能完全激活。
而主网上线确认时刻的区块数是5594，时间约为2018年12月13日北京时间15:40。
如果按0.5秒生产1个区块计算，主网启动后大概要过138小时（约5.5天）才能正式激活，也就是12月18日左右。
而赎回和转帐等操作是需要在主网激活后才能进行的，所以无论你决定在主网激活后进行什么操作，在这3天时间里都可以尽情投票，尝试了解各个侯选节点的理念和特点，也是非常有意思的，Telos 感谢你们的支持！

最后，请投**保持独立性**，坚守“**公平、公正、公开**”原则的 **Telos Canton** 一票，BP名称：**teloscantons**
再次感谢你们的支持！

### Telos Canton 团队