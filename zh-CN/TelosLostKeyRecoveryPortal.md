# Telos密钥丢失的恢复方法

你的密钥丢失或被盗了？ Telos希望确保正当的持币者在即将到来的Telos投放中能获得属于他们的TLOS代币。

Telos会以EOS ERC-20快照为基准，1:1比例发放TLOS代币（最高上限为40000个）。Telos的私钥与账户名与EOS创世快照一致。 不幸的是，这意味着那些在EOS创世之时或之后丢失或被盗密钥的用户，需要将他们原来的密钥转换成Telos链上的。 因此，我们正尝试让社区知道，在EOS创世时拥有账户的用户，在需要的时候可以修改他们在Telos上的密钥。

关键的修改替换手续需要在主网启动前完成。 因为Telos使用原始的ERC-20快照，所以我们能基于持有这些密钥的以太坊地址验证所有权，并且可以绕开在EOS启动后可能在账户上出现的任何网络钓鱼或密钥丢失。 我们有一个特殊的时间窗口，以帮助任何失去EOS账户的人能保持对新Telos账户的控制。

必须澄清，Telos只能在Telos链上保护丢失或被盗账户的权益。 可惜我们并没有权力去帮助那些丢失密钥的EOS账户。

## 方式一：

这个方式适用于任何曾为他们的EOS ERC-20代币做过映射，但后来私钥丢失或被盗的人。 这会适用于98%的用户，所以它可能也适合你。

你需要使用你在EOS创世快照上的以太坊地址，用这个地址在以太坊区块链上为一个信息签名。 这个信息包括了一个新的公钥，这个公钥可以用任何钱包生成，这里我们用了Sqrl（Telos本地钱包），示例如下。 Sqrl可以创建以EOS或者TLOS开头的公钥，先创建哪个都可以，顺序不重要。

请确保你保存了与你的公钥相关联的私钥。 有了私钥你才能使用你的账户！ 当你发送了信息后，请将你发送信息的以太坊地址和对应的EOS公钥发给我们。 我们将验证该信息并为你更改密钥。

请按照以下指引操作：

1. 从telosfoundation.io/downloads下载Sqrl钱包

2. 为新的Telos帐户生成新的密钥:
    
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_1.png" />
    </div>
    <p align="center">
      打开 Sqrl 钱包
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_2.png" />
    </div>
    <p align="center">
      选择 "Telos Testnet"
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_3.png" />
    </div>
    <p align="center">
      单击 "Create New Account - 创建新帐户"
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_4.png" />
    </div>
    <p align="center">
      输入您选择的帐户
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_5.png" />
    </div>
    <p align="center">
      生成公钥 - "所有者"权限
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_6.png" />
    </div>
    <p align="center">
      将"owner - 所有者"权限的公钥拷贝进入"active - 有效"权限公钥的输入框
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_7.jpg" />
    </div>
    <p align="center">
      将你的私钥保存到安全的地方！ 建议你用储存在线下。
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_8.jpg" />
    </div>
    <p align="center">
      创建帐户是没有必要的, 你只需要新的密钥!
    </p>
3. 访问: www.myetherwallet.com/signmsg.html
    
    - 登录并选择持有你的 EOS币的以太坊钱包。
    
    - 拷贝如下信息：
        
        As the cryptographically verified owner of ethereum address listed below ("Ethereum Address"), I attest that I did own the EOS tokens listed on the EOS ERC-20 snapshot associated with this address and that I hereby request that the public key for my account be changed to the new EOS public key below (“New EOS Public Key”) or the Telos Network address equivalent for my corresponding account on the Telos Network. I agree to release the Telos Network and its Members - as well as the members of any blockchain project that may subsequently use this same value snapshot in the future - from any claim arising from this request. The cryptographic signature of this document constitutes my legal digital signature in all jurisdictions.
        
        Ethereum Address: New EOS Public Key:
        
        <div align="center">
          <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_1.jpg" />
        </div>
        <div align="center">
          <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_2.jpg" />
        </div>
    - 在Ethereum Address和New Eos Public Key里面分别填入你的以太坊地址和对应的新EOS公钥。发送消息后，将你的以太坊地址和公钥信息发到我们的邮箱。

## 方式二：

这个方式是针对那些在创始快照之前没有在Block One注册过EOS ERC-20代币的用户。 Because you will need to enter your private ethereum keys, we are directing you to EOS Authority. They are a respected block producer and have developed a verified process that will work on the Telos network exactly as it does on the EOS network.

1. 访问EOS Authority网站：
    
    https://eosauthority.com/blog/how_to_generate_your_EOS_fallback_key_from_ethereum_private_key

2. Save those keys for your SQRL wallet account.

3. 主网启动后通过SQRL导入钱包。