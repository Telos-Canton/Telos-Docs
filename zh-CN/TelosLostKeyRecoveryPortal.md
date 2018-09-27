# Telos密钥丢失的恢复方法

你的密钥丢失或被盗了？ Telos希望确保正当的持币者在即将到来的Telos投放中能获得属于他们的TLOS代币。

Telos会以EOS ERC-20快照为基准，1:1比例发放TLOS代币（最高上限为40000个）。Telos的私钥与账户名与EOS创世快照一致。 不幸的是，这意味着那些在EOS创世之时或之后丢失或被盗密钥的用户，需要将他们原来的密钥转换成Telos链上的。 因此，我们正尝试让社区知道，在EOS创世时拥有账户的用户，在需要的时候可以修改他们在Telos上的密钥。

关键的修改替换手续需要在主网启动前完成。 因为Telos使用原始的ERC-20快照，所以我们能基于持有这些密钥的以太坊地址验证所有权，并且可以绕开在EOS启动后可能在账户上出现的任何网络钓鱼或密钥丢失。 我们有一个特殊的时间窗口，以帮助任何失去EOS账户的人能保持对新Telos账户的控制。

必须澄清，Telos只能在Telos链上保护丢失或被盗账户的权益。 可惜我们并没有权力去帮助那些丢失密钥的EOS账户。

## 方式一：

这个方式适用于任何曾为他们的EOS ERC-20代币做过映射，但后来私钥丢失或被盗的人。 这会适用于98%的用户，所以它可能也适合你。

你需要使用你在EOS创世快照上的以太坊地址，用这个地址在以太坊区块链上为一个信息签名。 This message will include a new public key that you can generate in any wallet you choose; we show examples here using the Sqrl, the native Telos wallet. Sqrl can create a public key that begins with either EOS or TLOS; the order doesn’t matter.

Be sure to save the private key associated with your new public key. This is how you will access your account! Once you send the message, please send us the Ethereum address and EOS public key you recorded. We will verify the message and change the keys.

请按照以下指引操作：

1. Download the Sqrl wallet from telosfoundation.io/downloads

2. Generate new keys for a new Telos account:
    
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_1.png" />
    </div>
    <p align="center">
      Open up the Sqrl wallet.
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_2.png" />
    </div>
    <p align="center">
      Select "Telos Testnet"
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_3.png" />
    </div>
    <p align="center">
      Click "Create New Account"
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_4.png" />
    </div>
    <p align="center">
      Enter your account name
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_5.png" />
    </div>
    <p align="center">
      Generate "Owner Public Key"
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_6.png" />
    </div>
    <p align="center">
      "Owner Public Key" into "Active Public Key" field
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_7.jpg" />
    </div>
    <p align="center">
      Copy/Paste your Keys to a safe place! Offline storage is recommended.
    </p>
    <div align="center">
      <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_8.jpg" />
    </div>
    <p align="center">
      Creating an account is not necessary, you just need your new keys!
    </p>
3. Go to: www.myetherwallet.com/signmsg.html
    
    - Sign in and select the Ethereum wallet that held your EOS tokens.
    
    - Copy/paste this message:
        
        As the cryptographically verified owner of ethereum address listed below ("Ethereum Address"), I attest that I did own the EOS tokens listed on the EOS ERC-20 snapshot associated with this address and that I hereby request that the public key for my account be changed to the new EOS public key below (“New EOS Public Key”) or the Telos Network address equivalent for my corresponding account on the Telos Network. I agree to release the Telos Network and its Members - as well as the members of any blockchain project that may subsequently use this same value snapshot in the future - from any claim arising from this request. The cryptographic signature of this document constitutes my legal digital signature in all jurisdictions.
        
        Ethereum Address: New EOS Public Key:
        
        <div align="center">
          <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_1.jpg" />
        </div>
        <div align="center">
          <img src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_2.jpg" />
        </div>
    - Email us your information so we can research your claim.

## 方式二：

This process is for people who never registered their EOS ERC-20 tokens with Block One prior to the genesis snapshot. Because you will need to enter your private ethereum keys, we are directing you to EOS Authority. They are a respected block producer and have developed a verified process that will work on the Telos network exactly as it does on the EOS network.

1. 访问EOS Authority网站：
    
    https://eosauthority.com/blog/how_to_generate_your_EOS_fallback_key_from_ethereum_private_key

2. Save those keys for your SQRL wallet account.

3. 主网启动后通过SQRL导入钱包。