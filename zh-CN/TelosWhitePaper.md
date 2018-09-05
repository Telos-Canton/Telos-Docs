# 橡果（Telos）白皮书 v1.3

<img align="center" src="./images/telos_logo.png" width="147px" height="159px" />

*一个可持续的去中心化 EOSIO 网络 作者：道格拉斯·泓恩（Douglas Horn）*

TELOS - 事物的终极目的。 （来自希腊语ΤΈΛΟΣ）

> “橡果的终极目的是成为一颗橡树。”——亚里士多德

**草案 1.2：2018年8月15日**

<!-- MarkdownTOC autolink=true levels=1,2,3 bracket=round bullets="-,*,+" -->

- [橡果（Telos）项目](#the-telos-project) 
  - [TELOS区块链](#the-telos-blockchain)
  - [Telos给你一个崭新开始](#a-fresh-start-with-telos)
- [Telos的优势](#the-telos-advantage) 
  - [对开发者](#for-developers) 
    - [允许拥有专利权的去中心化应用（DApps）](#proprietary-dapps-allowed)
    - [较低的DApp开发成本](#lower-cost-dapp-deployment)
    - [较少的网络停顿](#fewer-network-pauses)
    - [增强的安全性](#enhanced-security)
    - [由区块生产者运营的公共测试网](#public-testnet-operated-by-block-producers)
    - [TELOS/EOS主网兼容性](#teloseos-mainnet-compatibility)
  - [对于通证持有者](#for-token-holders) 
    - [所有的投票都有意义](#meaningful-voting-for-all)
    - [每个通证具有更高平等性](#higher-equity-per-token)
    - [开发者专注于创造价值](#developer-focus-builds-value)
    - [较低的通胀率](#lower-inflation)
    - [被盗通证的预激活解决方案](#pre-activation-resolution-of-stolen-tokens)
  - [对于区块生产者](#for-block-producers) 
    - [公平的支付模式](#equitable-payout-model)
    - [公平的投票/反投票权重](#equitable-voting--inverse-vote-weighting)
    - [智能合约加强对区块生产者的要求](#smart-contract-enforced-block-producer-requirements)
    - [节点维护的常规停机时间](#regular-downtime-for-node-maintenance)
- [TELOS令牌分配](#telos-token-distribution) 
  - [比较分配](#comparative-distribution)
- [ Eos 问题，Telos 解决](#eos-problems-telos-solutions) 
  - [Eos的问题以及Telos将怎样解决它们](#eos-problems-and-how-telos-will-solve-them) 
    - [问题：用户投票无关紧要 - 巨鲸统治网络](#problem-user-votes-don%E2%80%99t-matter-%E2%80%93-whales-run-the-network)
    - [问题：DAPP开发人员失去激励去使用网络](#problem-dapp-developers-are-disincentivized-from-using-network)
    - [问题：网络暂停风险](#problem-network-pause-risk)
    - [问题：备用BP没有适当地得到支付和定期测试](#problem-standby-bps-are-not-being-properly-paid-and-regularly-tested)
    - [问题：EOS RAM可能提高部署DAPPS的成本](#problem-eos-ram-prospecting-drives-up-the-cost-of-deploying-dapps)
    - [问题：Eos宪法未经批准](#problem-the-eos-constitution-is-unratified)
    - [问题：在启动时没有准备好裁决机构 ](#problem-adjudication-body-not-prepared-at-launch)
    - [Eos有高通胀](#problem-eos-has-high-inflation)
    - [Eos账户可能在3年后被没收](#problem-eos-accounts-can-be-forfeit-after-3-years)
- [Telos的基金会](#the-telos-foundation)
- [启动一个完整的网络](#launching-a-complete-network) 
  - [投票钱包](#voting-wallets)
  - [宪法](#governance)
  - [公投程序](#referendum-process)
  - [工人提案提交和投票程序](#worker-proposals-submission-and-voting-process)
  - [仲裁程序](#arbitration-process)
  - [仲裁机构](#arbitration-body)
  - [区块生产者执行](#block-producer-enforcement)
  - [中央信息中心](#central-information-hub)
- [Telos区块生产者最低要求](#telos-block-producer-minimum-requirements)
- [区块生产者支付](#block-producer-pay) 
  - [预计的Telos块生产者支付和美元价值](#projected-telos-block-producer-pay-and-usd-value)
- [在Telos网络里的仲裁](#arbitration-in-the-telos-network) 
  - [Telos仲裁程序](#telos-arbitration-process)
- [Telos被盗资金汇回程序](#telos-stolen-fund-repatriation-process) 
  - [Telos被盗资金汇回程序](#telos-stolen-fund-repatriation-process-1) 
    - [登记未被盗的地址](#registered-addresses-that-have-not-been-stolen)
    - [登记被盗的地址](#registered-addresses-that-have-been-stolen)
    - [来自销售的未认领的EOS令牌](#unclaimed-eos-tokens-from-token-sale)
    - [在EOS主网发布的交易所EOS TOKENS](#eos-tokens-on-exchanges-at-eos-mainnet-launch)
- [TELOS RAM投机预防](#telos-ram-speculation-prevention) 
  - [限制初始RAM分配](#limit-initial-ram-allocation)
  - [将RAM的增加与网络利用绑定](#tie-ram-increases-to-network-utilization)
  - [鼓励TELOS基金会帮助稳定价格](#encourage-telos-foundation-to-help-stabilize-price-swings)
- [Telos交易所请愿程序](#telos-exchange-petition-process) 
  - [交换TLOS令牌创建请愿程序](#exchange-tlos-token-creation-petition-process)
- [Telos是证券吗？](#is-telos-a-security)
- [问答](#telos-faq)

<!-- /MarkdownTOC -->

# 橡果（Telos）项目

一个可持续的去中心化 EOSIO 网络

Eos系统为新经济带来了了不起的承诺。 不幸的是，高度集中化破坏了这一承诺。 仅1.6％的Eos持有者拥有90％的令牌。 令牌所有权，治理和区块生产者BP选举都受到大量“鲸鱼”地址的影响，这些地址可以将Eos推向他们想要的任何方向，而不考虑大多数令牌持有者，开发者，甚至网络的整体健康状况。

Telos是基于相同EOSIO代码的一个替代网络，旨在解决Eos的关键问题。 Telos网络提供：

1. 经济去中心化 - 没有鲸鱼地址
2. 区块生产者BP和备用BP的公平薪酬结构
3. DApp开发人员友好的专有DApps和较低成本部署
4. 额外的令牌持有者保护和被盗令牌的预激活解决方案

> “EOS的梦想，在修复它的中心化问题之前不会实现。”– Juan M. Villaverde, Weiss Ratings

## Telos区块链

Telos forks EOSIO code into a new blockchain and updates the following elements:

- 通过将创世快照中每个地址的值限制为40,000 Telos（TLOS）令牌，消除少数“巨鲸”的极端经济实力。
  
  - 消除了巨鲸对区块生产者选举和令牌持有者投票的控制。
  - 如果他们同意发行TLOS并分发令牌，在交易过程中将请求在其快照时为其EOS所有者创建TLOS令牌，每个账户持有者的上限为40,000个。
  
  <img align="center" src="./images/ownership_distribution.png" width="448px" height="392" />

- 修改区块生产者（BP）和备用BP的支付模型以更好地保护网络。
  
  - 一个固定的21个BP加上30个基于投票产生的备用BP。
  - 在区块生产者和备用生产者之间平衡薪酬。 所有BP将被支付相同的金额，所有备用BP将被支付50％的BP费率。
  - 备用BP将定期（每3-7天）轮流进行一小段时间生成区块以取得报酬，以及证明其已准备好生产。
  - 无法连续生成180个区块的活跃BP将暂时被备用BP替换（在30分钟后，而不是Eos规则下的3小时后）。 3 hours under Eos rules). 
  - BP和备用BP因未生成/错过的区块而受到处罚。
  - 该模型将减少由于6个或更多BP变为不活跃而导致的网络暂停的发生率。
  - BP和备用BP在信息披露，惯例和硬件/连接方面具有明确的最低要求 - 无论投票如何，任何不符合最低要求的都将被禁止服务。
  - minimum will be prevented from serving regardless of voting.
  - BP/备用BP表现的统计数据将被公布，以使选民能够指向更可靠的BP。
- Telos代码审查/测试 
  - 区块生产者或由他们选出的机构将审查代码的安全性和价值。 
  - 新的代码版本将在主网络激活之前，在一个专用的测试网络上进行实时测试，这个专用网络由所有BP和备用BP维护。
  - BP和备用BP将根据专用测试网络的结果协调更新。
- Telos DApp开发人员可以将其DApp的原始代码部分指定为专有或开源。 （所有Eos DApps必须是开源的，这将限制许多潜在开发者的参与。）
- Telos将年度通胀率降至2.5％，而不是5％。
- Telos地址在不使用3年后不会被销毁。 Eos的这个功能是不公平和不必要的，不会在Telos中实施。 However, genesis Telos accounts created by the Eos genesis snapshot must be used at least once by their owners within one year to opt in to the system or they will be removed.

Telos将由参与Eos Mainnet Launch Group（EMLG）的Eos BP候选人联盟发起。 这个小组非常精通启动和运行主网的机制，因为它之前已经这样做了。

我们将分发一个全新的令牌TLOS，给Eos创世快照中列出的那些人。将稍做几点改动：

- 所有创世地址的上限为40,000 TLOS。
- 所有可以证明在发行/发射前被盗的地址都将被返回真正的所有者手中。
- New tokens will be generated to create the Telos Founders Rewards Pool (TFRP) to compensate the founders and the Telos Community Rewards Pool (TCRP) to compensate community members promoting Telos, and to fund the Telos Foundation – a promotional organization for funding work important to the Telos network outside the worker proposals system.
- 交易所同意买卖TLOS，并在快照时将TLOS通证分发给他们的EOS通证持有者，就可以请求由ABPs或BPs重新创建账户。每个账户持有人的上限为40,000。

由于来自希望接收令牌的客户的压力，交易所可能会列出TLOS，从而提供买卖方法。

Telos网络很可能更加稳定，因为区块生产者BP将通过广泛社区基于能力的投票而不是少量有从属关系的巨鲸进行选择。 另外，未能生产区块的区块生产者将在30分钟内（180个错过的区块）轮换出来，而不是3个小时。 此外，备用BP将被启用，并且需要每3-7天生成一个块以证明它们时刻准备就绪。 这种半定期计划为BP提供了维护和更新服务器所需的停机时间，从而降低了运营成本。 它还把更多的备用BP加入到治理中，因为备用BP的投票将影响BP投票。 这种方法意味着可以验证备用BP的能力和得到更高的网络弹性（可能减少网络暂停）。

开发人员可能更喜欢Telos系统，因为他们可能将某些DApp指定为专有，因此值得他们进行开发投资。 Telos网络将通过保持RAM可用性与网络需求相对应来降低部署成本，以减少早期参与者的RAM囤积。 这应该使部署DApps的成本低于在Eos上（的成本）。 在所有其他方面，Telos网络将与Eos主网软件保持兼容，以便DApps可以在任一网络上互换运行。

可以预期令牌持有者更加投入，因为与Eos相比，他们的投票更为重要。 Eos只有巨鲸的选票真的重要。 像Weiss Ratings这样的分析师可能会给予Telos更高的估值，因为他们已经警告集中化是Eos系统的一个严重问题，并建议对大型账户进行有限投票和吸收更多的BP - 这两者都是Telos做到了。 TLOS令牌供应将是EOS的五分之一到三分之一，具体取决于交易所参与。 鉴于所有这些优势，TLOS可能比EOS具有更大的价值。

## Telos - 一个崭新的开始

Eos主网的发布揭示了该系统的许多重要缺点。 我们很幸运从中学到了东西。 其中许多问题将及时得到解决。 Telos的优势是可以从新开始，可以直接处理这些问题，并在发布时立即解决最紧迫的问题。 Telos网络为在网络上运行EOSIO软件提供了新的开始，该网络专注于为DApp开发人员和令牌持有者提供明确而直接的价值。 最终，Telos可能会提供一个创新解决方案的测试平台，这个测试平台EOS主网可能会采用。 目前，Telos旨在成为一个有成本效益的，高度可靠的网络，用户可以免费加入，开发人员可以负担得起部署他们的DApps。

# Telos优势

Telos is a new network based on Eos. It offers many advantages over the Eos Mainnet.

对于开发人员

    允许专利的DApps
    降低DApp部署成本
    网络暂停较少
    增强安全性
    公共测试网由BP运营
    Telos / Eos主网兼容性
    

对于令牌持有人

    所有人的投票都有意义
    每个令牌的权益更高
    开发人员关注建立价值
    更低的通胀率
    被盗令牌的预激活解决方案
    

对于区块生产者

    公平的支付模式
    公平投票/反投票权重
    智能合约强制执行区块生产者要求
    节点维护的定期停机时间
    

* * *

## 对于开发者

Telos网络旨在为开发人员提供可靠，经济，管理良好的网络，以释放DApp。 Telos与Eos主网络相比具有以下优势：

### 允许专利的DApps

在Eos主网上运行的所有DApp代码都必须是开源的。 （Eos宪法：第VII条）Telos不会强迫开发人员开源他们的代码。

### 降低DApp部署成本

Telos网络将依实际使用比例来管理RAM需求。 这将限制早期RAM囤积并保持部署DApps的成本更加经济实惠。

### 更少的网络暂停

Telos网络使用区块生产者系统，该系统每天替换所有备用BP进行区块生产，以证明所有备用BP都能够在每次调用时生成区块。 该系统还允许任何不可运营的BP在错过30分钟（180个连续块）之后暂时换出，而不是在Eos主网上的3个小时。 这降低了由于6个BP在任何给定时间变为非活动状态而导致强制网络暂停的风险。

### 增强的安全性

Telos通过为Telos区块生产者添加强制性最低技术和信息披露要求，扩展了Eos网络的安全性。

所有Telos BP和备用BP都必须在BP专用测试网上有一个节点，在实施之前可以测试新的补丁*。 这通过在实施之前披露新的故障来增加网络安全性，并允许BP之间更好的更新协调以减少死链的事件。

（*已知漏洞的紧急安全补丁除外。）

### 公共测试网由BP运营

所有Telos区块生产者和备用BP都需要将一个节点贡献给与Telos主网相同的完整且开放的测试网络。 这有助于应用程序开发和测试。

### Telos / Eos主网兼容性

Telos网络运行与Eos主网相同的EOSIO软件，因此为Eos编写的DApp可以在Telos上运行。 Telos网络上唯一的代码改动，与BP如何被支付，选择和音不合规暂时被从服务中删除有关。 所有其他差异都来自于创世纪快照的修改，宪法变更和组织原则。

* * *

## 对于令牌持有者

Telos令牌（TLOS）优于EOS令牌：

### 所有人的投票都有意义

Telos创世令牌所有权限制了所有创世纪账户上限为40,000个TLOS令牌。 Telos基金会拥有的地址不能投票。 Telos基金会拥有的地址不能投票。 因此，Telos令牌所有权是任何加密货币网络中其中一个最均衡比例的。 与Eos成员相比，Telos成员在网络治理方面拥有更为平等的发言权。

### 每个令牌更高权益

每个EOS令牌代表Eos网络总值的1 / 1,000,0000,000。 由于Telos有较少的令牌，因此每个TLOS令牌代表Telos网络值的大约1 / 330,000,000 *。 对于相同数量的令牌，这是网络所有权百分比的3倍以上。

（*取决于为其EOS令牌所有者激活TLOS令牌分发的交易所总数。）

### 开发者专注建立价值

任何基于Eos的网络的价值最终都将反映网络对开发人员部署DApps的有用性。 Telos通过降低DApp部署成本和部署专有代码的能力为开发人员提供额外的价值。 随着时间的推移，这些功能可能使Telos网络对开发人员更具吸引力和更有价值。

### 更低的通胀

Eos通胀率定为每年5％。 Telos的目标是每年通胀2.5％。 TLOS令牌通胀率将比EOS低50％。

### 被盗令牌的预激活解决方案

Telos基金会和ABP将提供一份智能合约，允许任何被盗的EOS持有人在Telos主网启动之前证明其所有权。 这会将令牌返还给他们的合法所有者，并防止其他成员无意中购买可能因盗窃而被冻结的令牌。

* * *

## 对于区块生产者

区块生产者验证交易，提供网络安全性，并在区块链上执行关键的治理角色。 为了吸引最好的区块生产者加入Telos网络，我们已经实施了以下改进：

### 公平的支付模式

Telos区块生产者系统由21个BP和30个备用BP组成，根据用户投票排名。 每个区块生产者将获得与Telos 1％通胀相同的每日份额。 每个备用区块生产者（最多30个）将获得前21个块生产者收到的金额的一半。 每个备用区块生产者将每3-7天轮换一次生产区块以“获得他们的保留”并证明他们可以不断地履行其职责。 对于任何错过的区块，区块生产者将受到处罚，并将向Telos选民提供统计数据。

### 公平投票/反投票权重

在Eos投票系统中，巨鲸可以选举他们选择的任何区块生产者。 想要只支持他们自己的附属区块生产者的选民可以通过不投票给其他任何人来增加他们的选票价值 - 这会损害投票系统。 Telos没有巨鲸，因此区块生产者只需要说服TLOS令牌持有者的广泛集体，他们有很强的候选资格。

此外，Telos区块生产者投票是“反向加权”，这意味着如果您只投票给1或2个区块生产者，您的投票权重将低于您投票给30个BP的投票权。 这鼓励大多数Telos成员去了解更多关于区块生产者候选人。 并阻止那些只为自己及其分支机构投票的人。

<img align="center" src="https://latex.codecogs.com/gif.latex?Normal\%20Voting\cdot%20sin\left%20(%20\frac{\pi%20}{2}%20\cdot%20\frac{number\%20of\%20votes\%20cast}{maximum\%20number\%20of\%20votes\%20possible}%20\right%20)" />

<img align="center" src="./images/inverse_weighted_voting.png" width="422.5px" height="384px" />

### 智能合约强制执行对区块生产者的要求

Telos维持区块生产者的最低标准，使其成为合格的候选人。 这些标准基于安全性，服务器容量，信息披露以及参与公共和私有测试网。 从主网激活时起，这些标准将由智能合约强制执行，并且任何不符合要求的区块生产者候选人将无法成为BP，无论投票如何。 所有其他区块生产者候选人将自动上升等级填补队列，直到满足最低要求。

### 节点维护的定期停机时间

备用区块生产者将通过半定期安排每3天轮流生产几个小时来证明其可靠性。 这将使主要区块生产者经常有机会关闭节点以进行维护和升级。 这显著降低了操作成本。 该系统还确保所有备用BP随时准备履行其职责。

# Telos令牌分配

*Calculations & analysis by Ava Masucci*

Eos系统中令牌的分配是所有主要加密货币中最集中的其中一种。 而Telos分配是所有加密货币中最不集中的一种。

- 90％的EOS令牌被仅1.6％的地址控制。
  
  <img align="center" src="./images/telos_median_distribution_of_tokens.png" width="472px" height="428px" />
  
  更均匀的分配

最初将所有Telos地址的TLOS令牌数量限制为40,000，从根本上改变令牌分布，与EOS不同。方法如下：

- 删除86.5％的令牌供应或，865,000,000个令牌
- 减少在快照时注册的仅0.67％的地址或1,098个地址的持有的数量。
- 循环供应从约996,691,000 EOS减少到178,473,249 TLOS令牌。
- 假设另外78.6％（斐波那契水平）178,439,249将被重新加入货币供应量，因为为请求交易所创建的令牌，供应量将上升至约318,753,222。 
  - 将为ABP和Telos基金会创建额外的12,000,000个令牌，创造大约330,753,222个TLOS令牌的总货币供应量 - 约为Eos货币供应量的三分之一。
- 每个TLOS令牌将代表EOS令牌的网络权益的约3倍。

## 比较分布

将每个地址令牌数量限制在40,000改变了不到0.67％的注册地址。 以更大的数量限制令牌数量不会显著改变受影响的地址数量。

<img align="center" src="./images/percentage_of_eos_address_altered_vs_token_amount_cap.png" width="476" height="416px" />

<img align="center" src="./images/token_amount_capped_per_address_vs_percentage_of_tokens_altered.png" width="476px" height="412px" />

将令牌数量限制为40,000个会改变EOS令牌供应的约86％。 将令牌上限设置为更高的数字将使更少数量的令牌持有者获得更多权力。

<img align="center" src="./images/telos_and_eos_genesis_snapshot_token_distribution.png" width="700px" height="351px" />

# Eos Problems, Telos Solutions

## Eos Problems and How Telos Will Solve Them

We have been closely involved throughout the Eos mainnet launch process as voting and contribution members of the Eos Mainnet Launch Group (EMLG). This has been an awesome experience and experiment in decentralized decision-making, but it is marred by problems caused by Eos centralization and requirements of the Eos sale and process. By eliminating the extreme centralization inherent to Eos, Telos will solve many of these problems. Telos has more latitude to improve the tokenomics because it is not related to Block.one and did not raise any money through an ICO or presale. As a result, the Telos network may issue new TLOS tokens in any way it determines is best for the network.

### Problem: User votes don’t matter – Whales run the network.

Because of the huge economic disparity within the Eos network, and because only 21 block producers are designated to run the network and receive the large reward for doing so, whale token holders control the Eos system. They can simply vote in up to 30 affiliated block producers who will follow their demands. Independent block producers can be removed by giant EOS token holders at any time.

The Eos network has already seen that some block producers affiliated with whales are failing to produce blocks, missing necessary technical planning sessions, and failing to provide important information disclosures to voters. There is a danger that these whales may simply suck a large share of the 5% annual inflation out of the Eos network while providing minimal service because their voting power makes them practically unopposable.

**The Telos solution:**

There are no whales in Telos. Token holders will have a meaningful vote.

### Problem: DApp developers are disincentivized from using network.

The Eos Constitution specifies that all DApps and contracts on the Eos network must be open source. While this is appropriate for many contracts, it will limit the development of commercial DApps on the network. Developers must invest heavily in each new product they create; they rely on protection of their inventions to recoup these investments. If commercial DApps must be open source, developers will instead choose blockchains where their works can be protected. Additionally, the Eos mainnet is experiencing speculation on RAM reservations which will drive up the cost of deploying DApps on the network.

**The Telos solution:**

The Telos network will allow some applications to be designated as proprietary. Those who have received funds from the network (block producers, adjudicators, code contributors, etc.) within the last 6 months must designate any DApps as open source. In order to discourage speculation and lower the cost of deploying DApps, the Telos network will release RAM in concert with its actual DApp usage.

### Problem: Network pause risk.

The Eos network requires “2/3+1” consensus to operate. Without this number of block producers running, the network must be paused until 2/3+1 BPs are active. In practical terms, this means that if just 6 of the 21 active Eos BPs fail to produce blocks, then the network goes down. Standby BPs do not automatically replace missing BPs. In fact, BPs that have been voted in can’t be removed for nonperformance for at least 3 hours. Exacerbating this problem is the fact that Eos standby block producers are not regularly tested for their ability to step in and produce blocks. Further, there are no enforced minimum requirements for an Eos block producer. The only requirement is to receive votes. The danger is that if block producers go down, they cannot be replaced for three hours and the standbys who replace them may not be ready to fill in.

**The Telos solution:**

The Telos network regularly cycles in standby block producers to produce blocks (at least once every 3-7 days for each standby). This cycling system will also temporarily replace any active block producer who has not produced blocks in 30 minutes. This system has three distinct advantages for network resiliency: nonproductive block producers will be more rapidly replaced meaning it is far less likely 6 will be down at any given time, forcing a network pause; standbys will regularly prove their readiness; block producers will receive semi-scheduled downtime to maintain and update their equipment. Further, Telos uses a smart contract and ‘oracles’ to enforce block producer eligibility, ensuring that every BP meets minimum technical requirements.

### Problem: Standby BPs are not being properly paid and regularly tested.

Eos standby block producers are paid far less than the top 21 block producers and are rarely called upon to prove their capacity. Maintaining a top-notch node infrastructure is costly and without the need to prove their ability, standby block producers are likely to skimp on expensive improvements and maintenance—particularly because there are no enforced minimum requirements to meet. There is no ongoing mechanism for testing the readiness of standby block producers and primary block producers have no opportunities for scheduled downtime, which increases the challenges of maintaining the network. There is no way to be certain that the Eos mainnet will function properly in times of crisis.

**The Telos solution:**

Telos has a pool of up to 30 standby block producers selected and paid by voting rank. Standby block producers are paid half the rate of the top 21 block producers. To earn this pay, each standby will cycle into block production for a several hours every 3-7 days on a regular schedule to ensure that all paid standbys are able to step in to produce whenever needed. This scheduled rotation means that primary block producers have predictable maintenance windows to maintain their nodes, which lowers operational cost and increases reliability. Block producers and standbys that fail to produce blocks will be penalized. This system makes it difficult for groups to game the payment rewards system and actively discourages vote buying. Telos has minimum requirements (both technical and informational) enforced by smart contract that every block producer must meet, regardless of voting.

### Problem: Eos RAM prospecting drives up the cost of deploying DApps.

The Eos network launched with much more available RAM than the system required. Prospectors have taken to reserving this RAM early, likely without the intention to use it, but only to speculate on the rising price of RAM in the future. This speculation has led to a rapid increase in the price of RAM. When the DApps arrive that need this RAM, it is likely to be priced very high which makes deploying applications on Eos unnecessarily expensive.

**The Telos solution:**

Telos will launch with just 4GB of RAM. This will enable initial DApps and airdrops that people may wish to launch on the network but will not leave incentive for RAM speculation because RAM that prospectors reserve can easily be supplanted by new RAM entering the system. As a result, people are more likely to simply reserve the RAM that their expected DApps will require. Block producers will monitor DApp RAM usage and will add new RAM capacity when actual usage necessitates it. Additionally, the Telos Foundation will issue periodic guidance about what it believes is a reasonable RAM price and it may purchase RAM below that price and sell RAM above that price to limit the value of speculation. Further, any time the current price of RAM is more than 10% above the published guidance price, the Telos Foundation will sell RAM to developers at the published guidance price.

### Problem: The Eos Constitution is unratified.

The Eos Interim Constitution is self-defined as incomplete and requires revision and ratification before Eos can move forward with many of its legal and governance responsibilities. This is an expression of the founder’s personal values and Block.one’s need to keep the blockchain at arm’s length so as not to be deemed to have created a security. Due to the voting imbalances in EOS token distribution, the ratified constitution will likely support the needs of the whales over the needs of common users.

**The Telos solution:**

The Telos ‘constitution’ is known as the Telos Network Operating Agreement (https://github.com/TelosFoundation/tips/blob/master/TelosOperatingAgreement.md) will be valid and enforceable as written as of network launch. There is no need to wait for a revised or ratified version. Every Telos user will agree to this via Ricardian contract the first time they choose to use their Telos account. Telos users certainly have the right to amend the constitution whenever they deem this necessary. Paragraph 32 (Amending) empowers TLOS token holders to ratify or amend the constitution using the ‘ratifyamend’ contract that will be available upon network launch, and when this happens it is more likely to express the desires and aims of common Telos users. However, the network will not be deemed unratified if this does not happenimmediately.

### Problem: Adjudication body not prepared at launch.

Eos relies on an adjudication body to resolve all disputes. However, that body has not yet been fully formed or prepared. There are no funds provided to facilitate this. Therefore, problems such as repatriating stolen funds is a difficult one for block producers to solve.

**The Telos solution:**

Telos will initially resolve many judicial challenges prior to its mainnet launch. The Telos Arbitration Organization (TAO) will be ready to begin immediately. The TAO will accept the Telos Network Operating Agreement as complete and not requiring further ratification. The TAO will also have a clear and limited mandate as to which cases it can address. The Telos Foundation will initially fund the TAO so that it can resolve disputes immediately and remain free of conflict when adjudicating cases that involve block producers. Ongoing TAO funding will be paid from arbitration fees.

### Problem: Eos has high inflation

Eos inflation is 5% per year. This is too much and debases the currency. At 5% inflation the money supply doubles in just 14 years. Major world economies are currently aiming for 2% annual inflation. Eos inflation is distributed 1% to block producers and with the remainder divided based on block producer votes for worker proposals. Because whales can control voting, they have the ability to drive much of this inflation to their affiliates.

**The Telos solution:**

Telos will keep inflationlower, aiming for 2.5% per year. 1% will still go to 51 block producers and standbys (though divided more equally among them). The remainder will go to support adjudicators, development, and other functions. Because some DApps can be proprietary on Telos, the network will not need to pay as many grants to software developers.

### Problem: Eos accounts can be forfeit after 3 years

Under the Eos Constitution, any account that has not performed a transaction in 3 years is forfeit and its EOS tokens will be redistributed. Many long-term savers will be caught by this and unfairly lose their tokens. There is no method to appeal or recover tokens once lost. This is designed to protect system resources and keep people engaged with the network but it is far too draconian and seeks to solve a problem that has not been shown to actually exist.

**The Telos solution:**

Telos will not have any token forfeiture in its initial Telos Network Operating Agreement. If TLOS holders choose to amend the constitution to include one it will be their choice, not something imposed upon them. Telos members whose accounts are created by the genesis will be required to access their accounts at least once within the first year after activation of the Telos mainnet to signify their opting-in to the network and its operating agreement. Genesis accounts that do not use the network within one year will be deleted.

# The Telos Foundation

The Telos Foundation exists as a promotional and funding body to advance the network and provide support to network functions that are not funded in other ways. The aim of the Telos Foundation is to provide grants to groups promoting necessary network functions that cannot or are not supported by worker proposals. Early in the life of the network, worker proposals may be difficult to fund because the process is nascent and because there is little value in the early worker proposal fund while many projects need resources. Additionally, some groups may need funds that do not come from block producers. For example, the Telos Arbitration Organization may have a conflict of interest accepting initial funding from block producers, despite the fact that this initial funding is crucially important. By having the Telos Foundation fund these processes, this conflict is averted.

The Telos Foundation also aims to add a tool to fight RAM speculation and runaway RAM prices currently seen on Eos. The Telos Foundation will publish periodic price guidance on its view of reasonable RAM pricing. When the RAM price is below the guidance price it may use funds to buy RAM to raise the price and when the RAM price is above the guidance price it may sell previously purchased RAM to help lower the price. This will help to stabilize the price of RAM away from wide swings that encourage speculation. The Telos Foundation will also provide RAM grants to small independent developers in need of RAM to deploy DApps on the network, with a preference for open source DApps. This will help ensure that new innovators are not priced out of entering the system.

The intent of the Telos Foundation is to become a perpetual grant-funding organization with different voters than the block producers. The Telos Foundation will accomplish this through presenting worker proposals to the voters to reimburse grants that have been distributed. In this way, the community can decide whether to perpetuate the Telos Foundation or wind it down.

The Telos Foundation is a decentralized autonomous organization that votes via smart contracts using the Telos Foundation Voting Token (TFVT) – a token of no value that confers voting rights to its holders. In this way, the Telos Foundation can vote to decide disbursement of funds and election of its own public representatives. Voting tokens will be distributed throughout the Telos community during launch to encourage a wide range of voices in voting, drawn from a community of developers, block producers, writers, and other prominent community members. Each will receive 1 to 3 TFVTs. New tokens will be administered quarterly to members who are making a contribution to the Telos community. Voting is performed by smart contract with a simple majority by number of tokens voted carrying.

The Telos Foundation voters are drawn from active contributors to the Telos community—as selected by the existing Telos Foundation voters. The initial group of Telos Foundation voters will be draw from contributors to the Telos Network creation and launch. All Telos Foundation Voter Token holders will be publicly announced and their voting token addresses will be associated with their identities so that each voter’s voting record will also be publicly recorded on the blockchain.

**The Telos Foundation has no role in network governance. It does not vote its tokens or issue positions on voting matters or BP selection. Its sole functions are to provide funding to beneficial Telos projects that might otherwise go unfunded and to help stabilize the price of RAM on the network.**

Areas where the Telos Foundation may grant tokens include:

    - Compensation for those who contributed to the Telos launch success
    - Compensation for developers of valuable tools used on the Telos network
    - Initiating funding for the Telos Arbitration Organization
    - Reimbursing select exchanges for the cost of listing TLOS where necessary
    - Funding new tool creation
    - Funding advertising and marketing for the platform
    - Providing RAM grants to developers priced out of deploying by speculators
    - Any other function that promotes or secures the Telos network
    

Many of these cases may also be funded through worker proposals. The Telos Foundation will fund proposals that its voting members feel are not adequately funded through voting proposals.

A foundation funded with tokens and entrusted with promoting the network is a common enough entity in cryptocurrency. Many blockchain projects establish ongoing funding for their project’s version of the Telos Foundation. Telos has decided to leave these decisions in the hands of the block producers at any given time to best support the decentralized nature of the Telos network.

<img align="center" src="./images/the_telos_foundation.png" width="495.5px" height="162.5px" />

# Launching a Complete Network

Telos benefits from the lessons of the EOS mainnet launch. Some decisions made in that launch have proven to be problematic. Telos will improve on the launch by including all the tools necessary for the network to be a success.

## Voting Wallets

At Telos network launch, there will be approved voting wallets for users. Telos is working with wallet and tool developers including Scatter, Greymass, SimplEOS and Telos Lynx* to ensure that their wallets will work seamlessly on the Telos blockchain.

## Governance

Telos will have a full-force Telos Network Operating Agreement (like the EOS constitution) and all supporting governance documents upon launch addressing all areas of governance.

## Referendum Process

In addition to a full-force Constitution, Telos will have a constitutional referendum process upon launch in the form of a referendum voting contract. The referendum process will be clearly described and any Telos token holder may call the contract and propose a referendum vote.

## Worker Proposals Submission and Voting Process

Worker proposals are an important part of running the network. Upon Telos mainnet activation, there will be a well-documented, smart contract-based submission and voting process for worker proposals.

## Arbitration Process

The Telos white paper includes an overview of the arbitration process, which is driven by a multi-party smart contract.

## Arbitration Body

The Telos Arbitration Organization (TAO) will be active by the time the Telos mainnet activates. The Telos ABPs and others are actively seeking out qualified and interested personnel to lead the organization. To eliminate conflict of interest, the TAO will be initially funded by a grant from the Telos Foundation and thereafter, funded by arbitration fees and/or worker proposals.

## Block Producer Enforcement

Because elected block producers have the potential for enormous power in DPoS blockchains, it’s crucial that block producers swiftly police each other for infractions that, left unchecked, could threaten network security. Decentralizing the Telos voter base is an important step but without vigilance from elected block producers, centralization could emerge.

Telos will revise the Ricardian contract included in the regproducer smart contract that a member must execute in order to register as a block producer candidate. The existing contract asks block producer candidates to agree to certain provisions, but makes no suggestion about what should be done if these are violated. As a result, there has so far been no enforcement for infractions.

The revised Telos regproducer contract will clearly state proscribed actions along with penalties for violation—such as treating transactions preferentially, and will call on all other block producers to enforce. To facilitate this, there will be a smart contract that any block producer may execute documenting alleged violations on-chain and requiring all other block producers to vote to whether or not to enforce the required penalty. If a 2/3+1 majority votes to enforce, then the smart contract will carry out the enforcement immediately. No additional action will be required.

## Central Information Hub

Telos will host a variety of best-in-class blockchain tools at the TelosFoundation.io web site, giving Telos members and other interested parties a convenient hub for information. The website will be apolitical and show no favor to any block producer candidate over any other.

(* Scatter and Greymass do not endorse the Telos project. They are working with Telos to ensure compatibility for users of their products.)

# Telos Block Producer Minimum Requirements

All Telos block producers must meet a set of minimum requirements in order to serve, regardless of the number of votes they may receive. These requirements are both informational and technical. Compliance will be enforced by smart contract or some similar process to minimize subjectivity.

Each block producer candidate will provide at a minimum:

**Information:**

    - A telosbp.json file containing information regarding company formation, ownership, website, social media connections, key administrative contact, key technical contact.
    - Server connection information for at least 300 peers.
    

**Technical:**

    - Two mainnet nodes (one designated as block producer): Dedicated servers running no other processes, Intel Xeon processors with 8 cores, 128GB DDR3 ECC RAM, DDOS protection, 100Mbps internet connection with latency of under 500ms to testing node.
    - Two testnet nodes (public developer testnet and private BP testnet for new software): Intel i7 processors, 16GB DDR3 ECC RAM, DDOS protection, 100Mbps internet connection.
    

Each block producer’s compliance with the minimum requirements will be monitored by smart contracts and disinterested groups to ensure compliance. If the smart contract detects that a block producer is not in compliance it will:

    - Issue a notice of noncompliance to the block producer
    - After 24 hours, prevent the block producer from serving
      * All block producer votes will remain intact
      * As soon as the smart contract detects that the block producer is compliant again for 1 hour, it will become eligible to serve and will return to the rank dictated by the votes it has received.
    - If a block producer has remained out of compliance with the minimum requirements for more than 15 days, it will be unregistered as a block producer and will need to run regproducer again.
    - Compliance with some elements that cannot be verified by smart contract will be ensured through drafting of the Ricardian contract included in the regproducer contract that each block producer candidate must call.
      * This contract will clearly list actions that block producer candidates are prohibited from taking clearly linked to penalties that all other block producers must implement swiftly or be deemed in violation as well.
      * Strongly linking infractions and commensurate outcomes within the regproducer contract will allow swift and decisive action by other block producers, which is currently lacking in EOS mainnet governance.
    

It is the intent of the Telos ABPs that these minimums serve to keep block producers responsive. These minimum requirements are intended to be revised from time to time by a 2/3+1 vote of block producers. However, it is important to note that the Telos network is decentralized with no owners, managers, or fiduciaries and no system of governance outside the votes of block producers elected by the token holders. Future block producers are encouraged but by no means required to abide by any intent stated by the ABPs.

# Block Producer Pay

Block producers are a crucial component of any EOSIO network. There are 21 block producers validating the network at any time. There are also a number of standbys with the goal of being able to step in at any time to maintain network security should other block producers be knocked off the network.

Pay is very unequal between the top block producer and the bottom standby block producer. On July 3, 2018 the top block producer ‘bitfinexeos1’ earned 1,017 EOS (USD $8,960) while the lowest paid standby block producer ‘sheleaders21’ earned just 118 EOS (USD $1,040) a ratio of almost 9:1.

For the standby block producers to truly be able to step in at any time, they need to be able to afford to keep up with the very expensive technical requirements of enterprise-level servers, data centers, DDOS protection, and a staff to keep it all running. It is not easy to slide into this role at a moment’s notice.

At a pay ratio of 9:1, standby block producers will have a very hard time keeping up with the technical and staffing standards of the leaders. And because there is really no existing process in Eos for verifying the readiness of standby BPs, the ideal moneymaking strategy for an Eos standby block producer below #25 or so would be to run incapable nodes with the producer plugin and spend their entire budget on social media to get votes. This is not what the network needs standbys to do, but this is how they are incentivized by the pay structure.

The Telos pay structure addresses this by keeping pay at 2:1 between full-time elected block producers and standbys. This allows standby block producers to remain capable of keeping up with the elected block producers. The system also calls on them to step into block producing once every 3-7 days for 6 hours. The final mechanism is open to discussion, but one possible structure is as follows:

**Every elected block producer rotates out for 12 hours once per week.**  
**Every standby block producer rotates in for 6 hours once per 5 days.**

This reduces the cost of running servers for block producers because they can schedule weekly maintenance and updates and it forces standbys to be ready to truly protect the network. All block producers and standbys will be penalized for blocks not produced.

The following table envisions block producer and standby block producer pay at the outset of the network.

## Projected Telos Block Producer Pay and USD Value

| **USD-TLOS Price**             |             |      | $2.50        | $5.00          | $10.00         | $15.00         | $20.00         |
| ------------------------------ | ----------- | ---- | ------------ | -------------- | -------------- | -------------- | -------------- |
| **TLOS Money Supply**          | 331,753,222 | TLOS | $829,383,055 | $1,658,766,110 | $3,317,532,220 | $4,976,298,330 | $6,635,064,440 |
|                                |             |      |              |                |                |                |                |
| **Daily Inflation**            | 0.0027%     |      |              |                |                |                |                |
| **Total Daily Pay**            | 9,089.13    | TLOS | $22,722.82   | $45,446        | $90,891        | $136,337       | $181,783       |
| **BP Daily Pay(@ 21 BPs)**     | 252.48      | TLOS | $631         | $1,262         | $2,525         | $3,787         | $5,050         |
| **SBP Daily Pay(@ 30 SBPs)**   | 126.24      | TLOS | $316         | $631           | $1,262         | $1,894         | $2,525         |
|                                |             |      |              |                |                |                |                |
| **Monthly Inflation**          | 0.0833%     |      |              |                |                |                |                |
| **Total Monthly Pay**          | 276,317.26  | TLOS | $690,793.15  | $1,381,586.29  | $2,763,172.59  | $4,144,758.88  | $5,526,345.17  |
| **BP Monthly Pay(@ 21 BPs)**   | 7,675.48    | TLOS | $19,189      | $38,377        | $76,755        | $115,132       | $153,510       |
| **SBP Monthly Pay (@30 SBPs)** | 3,837.74    | TLOS | $9,594       | $19,189        | $38,377        | $57,566        | $76,755        |
|                                |             |      |              |                |                |                |                |
| **Annual Inflation**           | 1%          |      |              |                |                |                |                |
| **Total Annual Pay**           | 3,317,532   | TLOS | $8,293,831   | $16,587,661    | $33,175,322    | $49,762,983    | $66,350,644    |
| **BP Annual Pay(@ 21 BPs)**    | 92,153.67   | TLOS | $230,384     | $460,768       | $921,537       | $1,382,305     | $1,843,073     |
| **SBP Annual Pay(@ 30 SBPs)**  | 46,076.84   | TLOS | $115,192     | $230,384       | $460,768       | $691,153       | $921,537       |

(USD values are for reference only.)

# Arbitration in the Telos Network

The Telos ABPs intend to clarify their intention for the role and process of arbitration within the Telos network. It is their intention to create a functional Telos Arbitration Organization (TAO) prior to Telos mainnet activation.

In Telos, the primary role of arbitration is to resolve non-deterministic elements of smart contracts with arbitrators acting as human “oracles” to settle disputes. Secondarily, arbitrators will work with the parties to find an outcome when the actual actions of a smart contract are at odds with the intent and means documented in the Ricardian contract or when breach of contract is alleged. Arbitration is never meant to be used to resolve matters of stolen accounts through instructing block producers to freeze or modify accounts. This function is deemed to generally be moot since thieves can move tokens faster than accounts can be frozen and because EOSIO has robust security features that work to prevent theft. Owners bear responsibility for securing their own addresses.

This is the intent of the Telos ABPs. However, it is important to note that the Telos network is decentralized with no owners, managers, or fiduciaries and no system of governance outside the votes of block producers elected by the token holders. Future block producers are encouraged but by no means required to abide by any intent stated by the ABPs.

## Telos Arbitration Process

1. The TAO follows a set of core rules for Telos arbitration. Other rule systems (e.g. American Arbitration Association) may be layered on top of these if both parties agree.
2. The intent for TAO arbitrators is to act as a human “oracle” (data/information/decision source) for non-deterministic contract. Ideally, an arbitrator is appointed at the outset of a smart contract execution.
3. A case is submitted for arbitration via Dispute Arbitration Smart Contract (DASC) that includes information about the nature of the dispute, whether it is a new dispute or an appeal, and the arbitration fee. 
  - If a case has wiped out a member’s account, they may request no-fee arbitration TAO members may elect to waive fees or use grants from Worker Proposals or the Telos Foundation to cover these.
4. The arbitrator will request statements and information from both parties. 
  - The parties submit their statements and information to the arbitrator and each other.
  - The parties may submit rebuttals to another party’s statements and additional evidence to address opposition statements or evidence.
  - The arbitrator may ask any questions he or she deems necessary to determine an outcome.
  - The arbitrator renders a judgement based solely upon the evidence presented as it relates to the Telos Constitution and Rules and the terms of the smart contract in question. Where they differ, the intent documented by the Ricardian contract will be given more significance than the source code. This decision is transmitted to either the smart contract as an oracle data point, or to the block producers as an arbitrator order via the case’s DASC.
5. The arbitrator actions shall be executed directly (where allowed by prior agreement) or else submitted to block producers for execution. Such submission will be in the form of a transaction ordered to be executed on the blockchain along with arbitrator’s private key approval.
6. The block producers must execute the orders of the DASC within 12 hours.

- The intent for TAO arbitrators is NOT to attempt to refund funds lost through theft. Telos and EOSIO software have high level security protections. This is the best defense against theft. Thieves will move too quickly to defeat with arbitration. The process only risks further contagion to innocent parties who may acquire the stolen tokens. 
  - All funds stolen before the Telos launch begins that can provide cryptographic proof of ownership will be repatriated to original owners via assignment of new owner provided keys.

# Telos Stolen Fund Repatriation Process

In some cases during the Eos ICO and registration process, some addresses were incorrectly registered, left unregistered, or falsely registered in scams. The Telos ABPs intend to correct this situation to the extent possible before the network launch and provide TLOS tokens to those who should rightfully have them.

To accomplish this, the ABPs will seek to credit those who can prove, using cryptographic keys, that they are the true owners of lost or stolen tokens. This includes EOS tokens that were not originally registered prior to the snapshot. The following process is for repatriating funds to their rightful owners in advance of the Telos network launch.

## Telos Stolen Fund Repatriation Process

### Registered addresses that have not been stolen:

    1. No action required. Your TLOS tokens will be on the network
    

### Registered addresses that have been stolen:

    1. Address owner files claim, providing:
      * Stolen address
      * Cryptographic signature from Ethereum wallet as proof
      * A new EOSIO public key as half of a key pair that will control the account
    2. Address will be posted for contestation for 10 days (with no identifying information).
      * Any other user will have the opportunity to provide cryptographic evidence proving ownership.
    3. Uncontested addresses providing cryptographic proof of rightful ownership will have old public key replaced with provided new public key in the Telos genesis file.
    

### Unclaimed EOS tokens from token sale:

    1. Unregistered token owner files a claim providing:
      * Eos ICO purchase transaction hash
      * Cryptographic signature from purchasing Ethereum wallet as proof
      * A new EOSIO public key as half of a key pair that will control the account
    2. Addresses providing cryptographic proof of rightful ownership will have address and new public key inserted into the Telos genesis file.
    

### EOS tokens on exchanges at Eos mainnet launch:

    1. Telos ABPs have provided an exchange TLOS token creation petition process for exchanges to work with the ABPs to create tokens for their customers who held EOS at the time of the snapshot.
      * Exchanges must complete the process in order to receive new tokens to distribute to their customers.
    2. The Telos ABPs and block producers take no responsibility and will take no action for tokens held on exchanges.
    

The Telos ABPs intend to repatriate tokens that can be cryptographically proven to have been unregistered or stolen at the Ethereum registration or Eos voting stages under the rationale that this correction is possible and verifiable before the Telos network launches. We recognize that some losses were due to the ethereum registration process and the lack of approved consumer-grade voting wallets at Eos mainnet launch.

The Telos network will adopt base layer arbitration to protect token holders from theft. Not all forms of theft may be recoverable, but arbitrators will have the ability to call for block producers to freeze accused accounts for a limited amount of time upon presentation of evidence of theft. Telos block producers will have authority for specific actions to demand restitution in accordance with a duly processed arbitration contract. The arbitration contract and Telos Arbitration Organization will be active from the time of the network launch.

# Telos RAM Speculation Prevention

RAM speculation is a danger that has already emerged in Eos. Some speculation will always occur in healthy markets with scarce resources, however when speculation is out of control then it ties up valuable scarce resource and limits network availability. To maximize network utility and keep the Telos network a cost-effective place to deploy DApps, Telos will implement the following tactics meant to discourage rampant speculation.

- Limit initial RAM allocation
- Tie RAM increases to network utilization
- Encourage Telos Foundation to help stabilize price swings

## Limit Initial RAM Allocation

The Eos launch allocated 64GB of RAM on mainnet launch. This number is far, far more than any DApp on the network requires. To speculators this is an enormous land grab opportunity of a scarce resource at a very cheap price. Eventually this RAM will be valuable. This “RAM-grab” will lead to high speculation and a boom-bust cycle that works against network stability and makes deploying DApps a challenge to budget. This is a strike against the Eos network for serious developers and may serve to keep small innovators priced out of Eos altogether.

To encourage developers and avoid price swings, the Telos network will launch with 4GB of RAM. While this sounds low, it will be more than enough to support any real DApps or airdrops on the system. The low number serves as an incentive not to speculate on Telos RAM because new RAM can be released, reducing elevated values of existing speculation.

## Tie RAM Increases to Network Utilization

The Eos mainnet is debating how and when to change the RAM supply. Increasing available RAM will temporarily lower the price but will ultimately worsen speculation because there will be less potential RAM to release in the future.

The Telos network will tie new RAM releases to utilization figures. The initial proposed value is that when >50% of the network RAM is consistently in use over a set period of time, new RAM will be released. This will tie new RAM to network growth. The block producers will ultimately determine the network RAM supply via the ‘setram’ action.

## Encourage Telos Foundation to Help Stabilize Price Swings

The Telos Foundation is a non-governing body with independent governance. Its goal is to promote network growth through grants. It has an endowment for these grants which can also serve as a method to help discourage RAM speculation.

The Telos Foundation will publish regular guidance on the price of Telos RAM that it sees as reasonable in the professional opinion of experts hired by the Foundation to set the Telos published guidance price for RAM. When the price is lower than this guidance price, the Telos Foundation may buy RAM. When the price is higher, it may sell. This is intended to help stabilize the price. This approach naturally has its limits, but it is expected to aid in discouraging price gouging. Further, the Telos Foundation may elect to sell or lease RAM to developers at its published guidance price (regardless of current price) to encourage some developers to build on the system. When publishing its guidance price, the Telos Foundation will include published advice to the Telos block producers about when to release more RAM into the system. This decision will remain with the block producers, however. Any professionals hired by the Telos Foundation to set RAM pricing will be prohibited from trading Telos RAM on their own accounts.

To ensure that small innovators are not priced out of the network, the Telos Foundation will also issue some grants in the form of RAM to such developers. In such cases, it will favor open source DApps.

# Telos Exchange Petition Process

The Telos Appointed Block Producers (ABPs) create the following process to allow exchanges that listed EOS at the time of the snapshot to petition to have their Telos addresses funded through the creation of new TLOS tokens sufficient to provide TLOS tokens to EOS owners at the time of the snapshot (1:1 up to 40,000 TLOS per customer). The Telos ABPs agree to create tokens for every exchange that completes the process.

The intent of the Telos project is to provide TLOS to all EOS token owners at the time of the Eos snapshot (up to 40,000 per address or exchange customer). The Telos ABPs encourage future Telos block producers to honor this intent and to create tokens necessary for every exchange that follows the petition process. However, it is important to note that the Telos network is decentralized with no owners, managers, or fiduciaries and no system of governance outside the votes of block producers elected by the token holders. Future block producers are encouraged but by no means required to abide by any intent stated by the ABPs. Therefore, the ABPs launching the Telos network will only have the full control to process exchange petitions during the period between launch and activation. Upon activation, the decision of whether or not to create new tokens for any petitioning exchange will be up to a vote of 15 of the 21 elected block producers at the time.

The Telos ABPs have established an exchange outreach working group to contact all Eos exchanges and help guide them through the process during the launch period. It is important to stress that only during the Telos launch period is the creation of TLOS tokens for petitioning exchanged guaranteed by the ABPs.

## Exchange TLOS Token Creation Petition Process

1. The exchange and the Telos Exchange Outreach Working Group (TEOWG) initiate communications and each designate a representative for this case. Investment funds, online wallets, and similar institutions holding EOS tokens for multiple owners may also petition under this process.
2. The exchange signs a letter of intent to list TLOS tokens and provide them to their EOS token holders as of the time of the Eos snapshot with a cap of 40,000 TLOS tokens per account. This letter documents terms of new token printing including that the exchange will agree not to act as a block producer and not to vote tokens for which they are not the beneficial owners. (i.e. never to vote from their exchange holding addresses.) The exchange and/or Telos network may issue publicity about this development.
3. The exchange provides identification of all exchange-owned addresses on snapshot along with cryptographic proof of ownership and a statement that there are no other addresses under their control.
4. TEOWG provides current copy of current Telos node and client software and any additional support necessary to deploy.
5. Exchange provides anonymized list of account amounts at time of Eos snapshot as CSV file or similar.
6. TEOWG examines the exchange-provided accounts list and caps holdings of all accounts at 40,000 TLOS tokens.
7. The exchange and TEOWG agree on the total value of tokens to be created and the addresses (from the identified exchange-owned addresses) to which they will be sent.
8. The exchange publicly announces its upcoming listing of TLOS tokens and distribution to EOS owners with a launch date. (This may have occurred earlier but must occur by this point.)
9. TEOWG provides exchange’s petition along with documentation to Telos ABPs for review. The Telos ABPs will coordinate scheduling of TLOS token creation with the exchange’s release schedule.
10. The Telos ABPs vote to create tokens. The Ricardian contract of this transaction requires that the exchange must accept terms of not voting from these addresses and not operating a block producer candidate, and distributing all TLOS tokens to their customers as represented in the agreement.
11. The exchange enables trading of TLOS.

# Is Telos a Security?

Ultimately, it will be up to the agency that enforces securities law in each country to determine whether or not Telos’s TLOS tokens are considered a security—and therefore subject to regulation. However, the US Securities Exchange Commission has been known to set precedent in this area and recent statements by the SEC shine a very encouraging light on the question.

On May 7, 2018, William Hinman, SEC director of corporate finance spoke at the Yahoo Finance All Markets Summit and sought to clarify under what conditions a coin or token would be considered a security. Two core concepts emerged from his speech. First, a security is largely determined by the nature of its offering to the public—how it was sold, what representations were made, etc. Hinman’s second key point was that a coin or token that was initially sold in a way that would have been viewed as a security could eventually be sold in a way where it was not considered a security, based on decentralization and the lack of centralized entity controlling it. Hinman concluded:

**Based on my understanding of the present state of ether, the Ethereum network, and its decentralized structure, current offers and sales of ether are not securities transactions**

Based on both of these points, we the Telos ABPs endeavor to launch this useful network relying on Director Hinman’s statements that, just as Ethereum is not a security due to its decentralized nature TLOS would also not be considered a security since it is even more decentralized than Ethereum. Further, Telos never offered any tokens for sale or accepted any money whatsoever from investors.

We believe that, based on the determination of Mr. Hinman and the US SEC, the TLOS token should not be viewed as a security for two important reasons:

First, TLOS has never been offered in any type of ICO. TLOS is an entirely new token that will be created upon the Telos mainnet launch. The Telos network is recreating a modified ownership snapshot of the Eos token sale as a way to reward those who paid to have the open source EOSIO software created by Block.one. To be clear, all of the monies contributed to this ICO went to Block.one, none to the Telos network. The EOSIO software is open source and free to copy. The Telos ABPs have decided to reward the backers of Eos by granting tokens matching their Eos purchases, up to a capped amount per address, but there is no affiliation with Eos or Block.one. Telos did not sell anything so it is difficult to conclude that it ever offered a security.

Second, even if it should ever be concluded that TLOS tokens would have been a security, despite never having been sold or offered for sale, the point is rendered moot by the entirely decentralized nature of the Telos network. Telos has no owners, managers, or fiduciaries. The network is administered by independent network of validating node operators called block producers who are continuously elected through the smart contract voting of TLOS token holders. The TLOS token ownership is notably one of the most evenly distributed and decentralized of all cryptocurrencies. There is no evidence that any single entity will control even 0.5% of the Telos network.

The Telos network will be initially launched by appointed block producers (ABPs) who will initiate the network launch and will be granted TLOS tokens for their efforts. An entity referred to as the Telos Foundation will receive TLOS tokens as a way to provide funding grants for necessary network functions. At the time these TLOS token will be granted to these entities and the TLOS token holders at large, the tokens will have no par value because they derive their value from either the exchange price (at a time when they are not listed for trade on any exchange in the world) or by the network value (at a time when the network has neither been launched nor can conduct transactions).

Before the Telos network becomes live and open to transactions, the 6 ABPs will all relinquish their privileges and step aside for the 21 block producers elected from voting of at least 15% of all TLOS token holders. TLOS tokens will only attain value if the token holder-elected block producers in conjunction with the efforts of the members themselves create a working, valuable network.

Our understanding as ABPs is that, based on the comments of Mr. Hinman, published on the SEC web site, that TLOS tokens are not securities and our issuance of these no value tokens of ownership in a thoroughly decentralized network is not an offer of securities.

The ABPs are not attorneys and this should not be construed as legal advice. Frankly, this is largely unsettled law. However, Director Hinman’s statements are clear and have been published on the SEC web site, signaling that they are officially sanctioned. Based on this definition, it seems difficult to deem TLOS a security under the US SEC definition.

**NOTE: THIS IS NOT LEGAL OR SECURITIES ADVICE. IT IS OUR INTERPRETATION OF PUBLISHED STATEMENTS BY THE UNITED STATES SECURITIES EXCHANGE COMMISSION AS THEY MIGHT APPLY TO TLOS TOKENS. SEEK COUNSEL FROM YOUR OWN PROFESSIONAL ADVISORS BASED ON YOUR NEEDS AND JURISDICTION.**

# Telos FAQ

**Q: What is Telos?**

A: Telos is a new blockchain network based on EOSIO software.

**Q: What is the difference between Eos and Telos?**

A: Eos and Telos are both networks running the EOSIO software. Any smart contract that runs on one system should run equally well on the other. Telos has modified the Eos genesis snapshot and some rules to make the network more responsible to the majority of token holders, to be more attractive to DApp developers, and to generally run more responsively and sustainably.

**Q: What is TLOS?**

A: TLOS is the name of the token that reflects ownership in the Telos network. A TLOS token is like an EOS token except that there will be around 3X fewer TLOS tokens than EOS.

**Q: Are you taking away people’s EOS tokens?**

A: No. EOS holders will have the exact same number of EOS tokens on the Eos network as they ever had. That is what they purchased from Block.one. Telos is a new project based on the Eos network. The Eos source code is open source and freely available to fork. We have decided to give an equal number of TLOS tokens to every EOS token holder on the genesis snapshot, but capping values at 40,000 TLOS per genesis address. This means that there will be no whales created from the Telos genesis, although the total token ownership of any account is unlimited once the network launches.

**Q: Is Telos an airdrop?**

A: Telos is a completely new network using the same EOSIO operating software as Eos mainnet with a few small modifications. It is not an airdrop. However, the distribution of TLOS tokens is similar to an airdrop in that anyone who owned Eos tokens will receive new TLOS tokens at their addresses based on our genesis token distribution algorithm.

**Q: What exactly is the Telos genesis token distribution algorithm?**

A: Simply, it is that all Telos genesis addresses will receive the same number of tokens as their corresponding Eos addresses held in the genesis snapshot—up to a maximum of 40,000 tokens. Except for a few special cases: Addresses proven to have been stolen, phished, or misregistered, thereby depriving their rightful owners of them will be restored to new addresses controlled by their rightful owners; and new genesis tokens will be created to compensate the Telos Launch Group contributors and community members promoting the network, and to establish the Telos Foundation.

**Q: If you cap all accounts, how can EOS holders get TLOS from exchanges?**

A: The TLOS block producers have the ability to create new tokens by a vote of 2/3+1. The 6 ABPs agree to create new tokens for distribution for any exchange that can show EOS holdings on the snapshot and that agrees: to list TLOS; not to vote the exchange account; and to request and distribute only enough coins so that all EOS holders at the time of the snapshot receive their coins capped at 40,000 per account. The ABPs will have a process in place for exchanges to petition them to create TLOS tokens and promise to honor all valid petitions. (It will require a vote of 5 of the 6 block producers to accomplish this.) Once the Telos network activates and the elected block producers validate the network, it will take a vote of 15 of the 21 block producers to create new tokens for exchanges.

**Q: Why cap genesis addresses at 40,000 TLOS?**

A: The largest 1,050 Eos addresses control about 90% of EOS tokens and therefore completely control block producer selection, their voting, and ultimately the entire network. This makes the system dangerously centralized. By capping genesis addresses at 40,000 TLOS—approximately the 90th percentile of ownership—the Telos network will be one of the most evenly distributed major blockchains in existence. 162,930 addresses will have exactly as many TLOS as they did EOS. The total TLOS token supply will be lowered to approximately 200-400,000,000 TLOS tokens depending on how many exchanges petition to recreate their wallets.

**Q: Can Telos addresses ever have more than 40,000 TLOS?**

A: Yes. The 40,000 TLOS cap only applies at the network genesis. Addresses may hold any amount of TLOS thereafter.

**Q: Will you still require 15% of TLOS token holders to vote to launch the mainnet?**

A: Yes. However, with addresses capped and Telos Foundation addresses permanently excluded from voting, the number of total votes needed to launch will decrease. This will represent a much broader cross-section of individual TLOS token holders.

**Q: What is the difference between the Telos mainnet launch and activation?**

A: Telos mainnet launch is the process of the beginning to run the Telos network to allow votes to be cast for block producers and for network validation. Activation is the point when TLOS holders can begin transferring or otherwise controlling their tokens beyond just voting. Activation will commence 24 hours after 15% of TLOS token holders eligible to vote have voted for block producers and mainnet activation and at least 40 block producer candidates meet the minimum block producer requirements.

**Q: If exchange addresses cannot vote, will my TLOS tokens be able to vote if they are currently on an exchange?**

A: Once tokens are off the exchange and on your own Telos address, you can vote them. Individual owners cannot vote their tokens held on exchanges. Preventing voting from exchange accounts keeps exchanges from voting with customer tokens, which is against the Telos rules.

**Q: Will this hurt the Eos network?**

A: The Eos network will succeed or fail based on its own merits. We hope it succeeds, as we are all deeply invested in this project. However, the Eos mainnet release has revealed problems with the system that will be difficult to resolve on the Eos blockchain. “Whales” have shown that they generally just vote for their own block producer partners and even game the rewards system to harm other block producers— this may also be expected once worker proposals emerge. The Eos network is under the control of a few whale accounts. We offer a fresh approach where all token holders’ voices matter. Telos also hopes to provide a testbed for new ideas that may eventually be adopted by the Eos mainnet. In this way we hope to strengthen Eos.

**Q: If these changes will fix the network, why doesn’t Eos make them?**

A: Block.one sold EOS tokens in their tokensale. They accepted money for tokens and made certain representations. They can’t easily change the results of their sale—especially by reducing the tokens of their largest contributors, which is really the key change that fixes the system. Telos is a completely new system that never took money from nor made promises to anyone. We intend to build a network using the open source Eos software (that we all helped pay for) to create an entirely new network that better represents the true purpose of Eos.

**Q: Can I buy and sell TLOS tokens? What are they worth?**

A: TLOS tokens will not gain value until the Telos mainnet launches and they are able to be traded. In practical terms, TLOS will gain real value when exchanges accept them to trade against other cryptocurrencies. We expect that this will happen because exchange customers will demand that they be given access to their tokens. The technical requirements for listing TLOS will be identical to EOS so we expect little resistance on that point. Once tokens are freely trading on exchanges they will find their value based on supply and demand. The TLOS token supply will be between one-fifth and one-third that of EOS, and the Telos network should be as good as or better than Eos. Telos will also not have any “whale” addresses which often are responsible for price manipulations in other coins.

**Q: Are you selling TLOS tokens?**

A: We are not selling any TLOS tokens. We will use the Eos Snapshot with the following changes: 1) Capping all addresses at 40,000; 2) Creating a process for exchange addresses to petition the BPs to create TLOS tokens for their EOS snapshot owners by listing and distributing TLOS tokens (up to 40,000 per account holder); 3) Providing new public keys to EOS token holders who can prove that their tokens were stolen or misregistered; 4) Adding 6M new tokens to form a Telos Founders Reward Pool, 1M new tokens to form a Telos Community Rewards Pool, and 6M TLOS tokens to the Telos Foundation Ltd, to support network needs that cannot otherwise be funded. These tokens currently have no value and will only gain value if the Launch Group and Telos Foundation can create a valuable network. The Telos Foundation pledges to never vote its tokens.

**Q: Who are you and why are you launching Telos?**

A: We are a group of Eos block producer candidates who have contributed to the system, run testnets, and taken part in the Eos Mainnet Launch Group that voted to unanimously launch the mainnet. We believe in the promise of Eos, but we have come to be concerned that the current system is deeply flawed due to the overwhelming power of Eos token holders with enormous holdings. We hope that Eos can overcome this problem, but in the meantime, we want to launch a new, more decentralized network using the Eos technology.

**Q: Can Eos block producers also be Telos block producers?**

A: Absolutely! We hope they will since they know how to run EOSIO nodes well. Anyone who meets the minimum requirements for a Telos block producer may submit themselves for voting.

**Q: Can developers make their code proprietary?**

A: Yes. If the developer has not accepted payment as a block producer, code reviewer, or worker proposal recipient in the past six months, they can designate the original code in a DApp as proprietary. Any underlying open source code that the DApp is built upon will remain open source, of course. By contrast, all smart contracts running on the Eos network must be open source according to the Eos Constitution.

**Q: What if Telos users don’t want to use proprietary software on the blockchain?**

A: Each smart contract will designate if portions of its code are proprietary. Telos members will be able to choose whether or not they wish to work with proprietary smart contracts or only open source contracts.

**Q: When will the Telos mainnet launch?**

A: The Telos Launch Group will hold a series of “go/no-go” votes about launching the Telos mainnet starting on September 28, 2018. To vote “go” each Contributor will need to agree that a series of promised elements (e.g. arbitration, governance, ratification, plus all technical requirements) have been delivered sufficient to launch a complete and successful network. Once a majority “go” vote is reached, the network will be launched by the ABPs until it receives both 15% of all outstanding Telos votes (Telos Foundation addresses), and at least 40 Telos block producer candidates who meet the minimum requirements. At this point the ABPs will resign any special powers and 24 hours later the Telos mainnet will activate for transactions. In other words, we will wait for a groundswell of support from both the original Eos token holders and a group of highly qualified technical block producer candidates. We believe that this will indicate a true mandate for the Telos network.

**Q: How are Telos block producers paid?**

A: Telos will have 21 active block producers and up to 30 standby block producers sharing the 1% TLOS inflation. Each block producer will be paid the same flat rate and each standby will be one half of that rate. All will receive pay deductions for missed blocks.

**Q: Will the team launching Telos take a fee for its service?**

A: Launching the Telos network is an expensive and time-consuming venture. The people launching Telos include block producers, developers, social media marketers, arbitrators, and others working together in a largely decentralized way. Members of the Telos Launch Group will be compensated in the TLOS genesis file. A Telos Founders Reward Pool (TFRP) will be created in the Telos genesis file containing 6M TLOS (about 1.8% of the expected money supply). This fund will be distributed among members of the Telos Launch Group – an open-membership group established to create and launch the Telos network – based on tasks performed by members. The exact method of TFRP distribution is yet to be determined but will be formalized prior to network launch.

**Q: You say that Telos won’t have any “whales” but aren’t the TFRP recipients and Telos Foundation going to become whales?**

A: The Telos Foundation will never vote its tokens. TFRP funds will be broadly distributed among contributors in a manner to be determined soon. Distributions over a certain amount will unlock evenly over a 3-year period similar to how Block.one’s tokens vest. No TFRP recipient will be able to vote itself into the block producer ranks without the help of many TLOS token holders.

**Q: Why are TLG members being compensated?**

A: Members of the Telos Launch Group are taking a central role in creating and launching the Telos network. They are bearing the costs and contributing the effort to bring the network to life. To compensate their work and defray cost they incur, they are being granted new genesis tokens on the Telos blockchain distributed from the Telos Founders Reserve Pool. These tokens are of zero value at the genesis and will only gain value if the TLG, Telos Foundation, and other participants can launch a valuable network. This approach is in line with bounty programs common in cryptocurrency launches. The total amount of compensation for the many founders/bounty recipients is ~1.8% of the expected Telos token supply, which is a low number for cryptocurrency projects where large amounts of work are required and no funding has been sought.

**Q: What is the Telos Foundation?**

A: The Telos Foundation is a promotional arm of the Telos Network. Prior to the Telos mainnet launch, the Telos foundation will organize technical, informational, and marketing efforts to advance the Telos network. The Telos Foundation will manage the Telos genesis file subject to validation of the ABPs. Immediately upon the mainnet launch, the Telos Foundation will cede its authority to the ABPs to be governed by the Telos Constitution and voting rules.

After mainnet launch the Telos Foundation will function as an independent promotion and funding body for the Telos network. Its function will be to pay for projects that are not selected for worker proposals or that cannot yet be funded due to inadequate funds. (Particularly early in the life of the network.) The Telos Foundation may apply for worker proposal funds to reimburse funds dispersed as the goal is to create an ongoing fund that is not depleted. It will also seek to stabilize RAM prices by regularly publishing a guidance price and buying below that price, selling above it, and offering RAM for sale or lease to bona fide developers seeking to develop on the network.

The Telos Foundation is a decentralized organization that votes on its own issues via smart contract. It does not serve or seek any official governance position and will remain neutral on block producer candidates and proposals. Addresses owned by the Telos Foundation will never vote.