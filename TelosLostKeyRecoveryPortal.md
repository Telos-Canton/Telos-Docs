# Telos Lost Key Recovery Portal

Were your keys lost or compromised on EOS? Telos wants to make sure the proper owners receive their TLOS tokens in our upcoming Telos sharedrop!

Telos will give TLOS tokens 1:1 based on the original EOS ERC-20 snapshot (up to 40,000 per account) using the same keys and account names as the EOS genesis. Unfortunately, this means that anyone whose keys were lost or compromised at that time or since that time will also need their keys replaced on the Telos chain. For this reason, we’re working to alert EOS genesis token holders that Telos will allow them to revise their keys where necessary.

The key replacement process needs to occur BEFORE the Telos mainnet launches. Because Telos is using the original ERC-20 snapshot, we can verify ownership based on the Ethereum address that held those keys and can bypass any phishing or other key loss that may have happened to accounts after EOS launched. We have a special window of time in which to help anyone who lost their EOS accounts to maintain control of their new Telos accounts.

To be clear, Telos can only protect lost or compromised genesis accounts on the Telos blockchain. Unfortunately, we have no power to aid lost key issues on EOS accounts.

## PROCESS 1

This is the process for any users who registered their EOS ERC-20 tokens but later lost their keys or had them compromised. This will apply to 98% of users so it is probably the right one for you.

You will sign a message on the Ethereum blockchain from the same address that held your EOS tokens at the snapshot. This message will include a new public key that you can generate in any wallet you choose; we show examples here using the Sqrl, the native Telos wallet. Sqrl can create a public key that begins with either EOS or TLOS; the order doesn’t matter.

Be sure to save the private key associated with your new public key. This is how you will access your account! Once you send the message, please send us the Ethereum address and EOS public key you recorded. We will verify the message and change the keys.

Follow the instructions below:

1. Download the Sqrl wallet from telosfoundation.io/downloads

2. Generate new keys to send us:

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_1.png">
    </div>

    <p align="center">Open up the Sqrl wallet.</p>

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_2.png">
    </div>

    <p align="center">Select "Telos Testnet"</p>

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_3.png">
    </div>


    <p align="center">Click "Create New Account"</p>

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_4.png">
    </div>

    <p align="center">Enter your account name</p>

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_5.png">
    </div>

    <p align="center">Generate "Owner Public Key"</p>

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_6.png">
    </div>

    <p align="center">"Owner Public Key" into "Active Public Key" field</p>

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_7.jpg">
    </div>

    <p align="center">Copy/Paste your Keys to a safe place! Offline storage is recommended.</p>

    <div align="center">
        <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/step_8.jpg">
    </div>

    <p align="center">Creating an account is not necessary, you just need your new keys!</p>

3. Go to: www.myetherwallet.com/signmsg.html

    - Sign in and select the Ethereum wallet that held your EOS tokens.

    - Copy/paste this message and add your Ethereum public key and your new Telos Public Key (or an EOS key you want to use):

        As the cryptographically verified owner of ethereum address listed below ("Ethereum Address"), I attest that I did own the EOS tokens listed on the EOS ERC-20 snapshot associated with this address and that I hereby request that the public key for my account be changed to the new EOS public key below ("New EOS Public Key") or the Telos Network address equivalent for my corresponding account on the Telos Network. I agree to release the Telos Network and its Members - as well as the members of any blockchain project that may subsequently use this same value snapshot in the future - from any claim arising from this request. The cryptographic signature of this document constitutes my legal digital signature in all jurisdictions.<br>
        Ethereum Address:<br>
        New EOS Public Key:

        <div align="center">
            <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_1.jpg">
        </div>

        <div align="center">
            <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_2.jpg">
        </div>
    <p align="center">Enter your own Ethereum address where you held your EOS tokens in "Ethereum Address" and your new SQRL public key into "New EOS Public Key"</p>
    
    <div align="center">
            <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_3.eb955e94.png">
        </div>
    <p align="center">Log into the wallet that has your Ethereum account where your EOS tokens where held.</p>    
        
    <div align="center">
            <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_4.e942d25d.jpg">
        </div>
    <p align="center">Sign the pasted message with the Ethereum address and new Telos Public Key (or an EOS key you want to use).</p>
    
    <div align="center">
            <img width="620" src="https://raw.githubusercontent.com/Telos-Canton/telos-docs/master/images/recovery/ether_screenshot_5.1c820298.jpg">
        </div>
    <p align="center">Copy this Signature text and send it in the form below</p>
    
    - Email us your information so we can research your claim.

## PROCESS 2

This process is for people who never registered their EOS ERC-20 tokens with Block One prior to the genesis snapshot. Because you will need to enter your private ethereum keys, we are directing you to EOS Authority. They are a respected block producer and have developed a verified process that will work on the Telos network exactly as it does on the EOS network.

1. Go to the EOS Authority web site:

    https://eosauthority.com/blog/how_to_generate_your_EOS_fallback_key_from_ethereum_private_key

2. Save those keys for your SQRL wallet account.
3. Import wallet through SQRL once network launches.
