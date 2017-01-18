##########
EARN ETHER 
##########

.. _sign-in:

***************************
Sign in (become a referral)
***************************

You need to sign in only once. 

**Video:**

`The Million Ether Smart Contract - sign in instructions (7:24) <https://youtu.be/0HR4N9lEc2I>`_

**Signing in requires 2 steps:**

1. Start watching the MillionEther smart contract.
2. Sign in using a referral link (address)

**Requirements:**

1. Ethereum address with at least 0,003 ether needed to pay the gas cost (Ethereum blockchain commission for making transactions) `Buying ether instructions <http://ethereum.stackexchange.com/a/2071/2919>`_.
2. `EthereumWallet <https://github.com/ethereum/mist/releases>`_  installed (alternatively you can use other popular clients like `Metamask <https://metamask.io/>`_ or `MyEtherWallet.com <https://www.myetherwallet.com/>`_). `EthereumWallet installation instructions <https://medium.com/@attores/step-by-step-guide-getting-started-with-ethereum-mist-wallet-772a3cc99af4#.j30bpfush>`_.




**1. Start watching the MillionEther smart contract.**

- In EthereumWallet go to Contracts, scroll down and click Watch contract button.

.. image:: /img/watch_contract.png

- copy-paste the contract address:

.. code-block:: none

	0x15dbdB25f870f21eaf9105e68e249E0426DaE916 

- copy-paste the contract JSON INTERFACE:

.. code-block:: json

	[{"constant":false,"inputs":[{"name":"newDelayInSeconds","type":"uint32"},{"name":"newCharityAddress","type":"address"},{"name":"newImagePlacementPriceInWei","type":"uint256"}],"name":"adminContractSettings","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"emergencyRefund","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"},{"name":"priceForEachBlockInWei","type":"uint256"}],"name":"sellBlocks","outputs":[{"name":"","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"}],"name":"getAreaPrice","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"x","type":"uint8"},{"name":"y","type":"uint8"}],"name":"getBlockInfo","outputs":[{"name":"landlord","type":"address"},{"name":"imageID","type":"uint256"},{"name":"sellPrice","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"},{"name":"imageSourceUrl","type":"string"},{"name":"adUrl","type":"string"},{"name":"adText","type":"string"}],"name":"placeImage","outputs":[{"name":"","type":"uint256"}],"payable":true,"type":"function"},{"constant":false,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"}],"name":"buyBlocks","outputs":[{"name":"","type":"uint256"}],"payable":true,"type":"function"},{"constant":true,"inputs":[{"name":"userAddress","type":"address"}],"name":"getUserInfo","outputs":[{"name":"referal","type":"address"},{"name":"handshakes","type":"uint8"},{"name":"balance","type":"uint256"},{"name":"activationTime","type":"uint32"},{"name":"banned","type":"bool"},{"name":"userID","type":"uint256"},{"name":"refunded","type":"bool"},{"name":"investments","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"userID","type":"uint256"}],"name":"getUserAddressByID","outputs":[{"name":"userAddress","type":"address"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"getMyInfo","outputs":[{"name":"balance","type":"uint256"},{"name":"activationTime","type":"uint32"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"getStateInfo","outputs":[{"name":"_numUsers","type":"uint256"},{"name":"_blocksSold","type":"uint16"},{"name":"_totalWeiInvested","type":"uint256"},{"name":"_numImages","type":"uint256"},{"name":"_setting_imagePlacementPriceInWei","type":"uint256"},{"name":"_numNewStatus","type":"uint256"},{"name":"_setting_delay","type":"uint32"}],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"withdrawAll","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"referal","type":"address"}],"name":"signIn","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"imageID","type":"uint256"}],"name":"getImageInfo","outputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"},{"name":"imageSourceUrl","type":"string"},{"name":"adUrl","type":"string"},{"name":"adText","type":"string"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"charityBalance","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"charityAddress","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"violator","type":"address"},{"name":"banViolator","type":"bool"},{"name":"pauseContract","type":"bool"},{"name":"refundInvestments","type":"bool"}],"name":"adminContractSecurity","outputs":[],"payable":false,"type":"function"},{"inputs":[],"payable":false,"type":"constructor"},{"payable":false,"type":"fallback"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"newUser","type":"address"},{"indexed":false,"name":"invitedBy","type":"address"},{"indexed":false,"name":"activationTime","type":"uint32"}],"name":"NewUser","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"fromX","type":"uint8"},{"indexed":false,"name":"fromY","type":"uint8"},{"indexed":false,"name":"toX","type":"uint8"},{"indexed":false,"name":"toY","type":"uint8"},{"indexed":false,"name":"price","type":"uint256"}],"name":"NewAreaStatus","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"fromX","type":"uint8"},{"indexed":false,"name":"fromY","type":"uint8"},{"indexed":false,"name":"toX","type":"uint8"},{"indexed":false,"name":"toY","type":"uint8"},{"indexed":false,"name":"imageSourceUrl","type":"string"},{"indexed":false,"name":"adUrl","type":"string"},{"indexed":false,"name":"adText","type":"string"}],"name":"NewImage","type":"event"}]

- copy-paste contract name: 

.. code-block:: none

	My Million Ether

.. image:: /img/million_ether_contract.png 

- click ok

You now should be able to see My Million Ether contract in Contracts section.


**2. Sign in using a referral link (address)**

- From your web browser copy your referral's address and paste it into referral field (make sure there are no whitespaces).

.. image:: /img/ref_in_browser.png 

.. note::

	Alternatively your referral's address is everything after slash: themillionetherhomepage.com/**0x5dcd0da5e8506.........fe0c1d4f60a6c724918**

- Go to Contracts -> My Million Ether -> Write to contract -> Select function -> Sign In.

.. image:: /img/sign_in.png 

- Click Execute and confirm transaction.

.. image:: /img/confirm.png 

.. note::

	The only ether you pay here is the gas price (Ethereum blockchain commission).

.. note::

	Your referral link is themillionetherhomepage.com/ + your public ethereum address. You can compose it yourself, but it is activated through sign in procedure only. 

.. image:: /img/activation_time.png 

.. note::

	If you receive **“It seems this transaction will fail, it may consume all the gas you send”** than check your referral's activation time. Go to Contracts -> My Million Ether -> Read from contract -> Get User Info. Copy-paste your referral's link and check the activation time. If the referral is not active yet, just wait for the :ref:`activation time<activation>` and try again.

Now you can share your link and start earning ether!



*************
Invite people
*************

**Video:**

`The Million Ether Smart Contract - sign in instructions (7:24) <https://youtu.be/0HR4N9lEc2I>`_

**1. Sign in if you haven't yet** - :ref:`Sign in <sign-in>` 


**2. Compose your personal link.**

In any text editor copy-paste **http://themillionetherhomepage.com/** and your address (the one you used to sign in) right after the last slash with no whitespaces.

.. image:: /img/compose_link.png

Now you can use this link to invite other people to participate. Share this link on a blogpost, social networks or send it by email to your friends. And you are now now able to :ref:`buy pixels and place ads<buy>`

.. note::

	Keep your activation time in my mind. You can start sharing your link but a person who tries to sign in with it will have to wait until your account activates. To check your activation time go to Contracts -> My Million Ether -> Read from contract -> Get my info -> Activation time. :ref:`More on activation time.<activation>`


********************
Withdraw your reward
********************

**1. Check your balance**

- Go to Contracts -> My Million Ether -> Read from contract ->  Get user info and paste your address.

.. image:: /img/check_balance.png 


**2. Withdraw**

- Go to Contracts -> My Million Ether -> WRITE TO CONTRACT -> Select function -> Withdraw All

.. image:: /img/withdraw.png 

- Click Execute and confirm transaction. 

In a couple of minutes (depending on block mining speed) your should be able to see your funds in your wallet. 

.. note::

	Make sure to have at least 0,003 ether on your account as even withdrawing funds requires a little ammount of gas.