##############################
Earn ether (become a referral)
##############################

.. _sign-in:

*******
Sign in
*******

You need to sign in only once. 

**Signing in requires 2 steps:**

1. Start watching the MillionEther smart contract.
2. Sign in using a referral link (address)

**Requirements:**

1. Ethereum address with at least 0,1 ether, needed to pay the gas cost (Ethereum blockchain commission for making transactions) `Buying ether instructions <http://ethereum.stackexchange.com/a/2071/2919>`_.
2. `EthereumWallet <https://github.com/ethereum/mist/releases>`_  installed (alternatively you can use other popular clients like `Metamask <https://metamask.io/>`_ or `MyEtherWallet.com <https://www.myetherwallet.com/>`_). `EthereumWallet installation instructions <https://medium.com/@attores/step-by-step-guide-getting-started-with-ethereum-mist-wallet-772a3cc99af4#.j30bpfush>`_.




**1. Start watching the MillionEther smart contract.**

- In EthereumWallet go to Contracts, scroll down and click Watch contract button.

.. image:: /img/powered_by_ethereum.png

- copy-paste the contract address: todo

.. code-block:: none

	0x3a02afaabf963f7c37da52835ba89acdd92992cd 

- copy-paste the contract JSON INTERFACE: todo

.. code-block:: json

	[{"constant":false,"inputs":[],"name":"admin_removeContract","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"violator","type":"address"},{"name":"newStatus","type":"bool"}],"name":"admin_freezeUser","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"emergencyRefund","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"newCharityAddress","type":"address"}],"name":"admin_setCharityAddress","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"x1","type":"uint8"},{"name":"y1","type":"uint8"},{"name":"x2","type":"uint8"},{"name":"y2","type":"uint8"},{"name":"priceForEachBlockInWei","type":"uint256"}],"name":"sellBlocks","outputs":[{"name":"","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"x1","type":"uint8"},{"name":"y1","type":"uint8"},{"name":"x2","type":"uint8"},{"name":"y2","type":"uint8"}],"name":"getAreaPrice","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"x","type":"uint8"},{"name":"y","type":"uint8"}],"name":"getBlockInfo","outputs":[{"name":"landlord","type":"address"},{"name":"imageID","type":"uint256"},{"name":"sellPrice","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"getMyBalance","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"x1","type":"uint8"},{"name":"y1","type":"uint8"},{"name":"x2","type":"uint8"},{"name":"y2","type":"uint8"},{"name":"imageSourceUrl","type":"string"},{"name":"adUrl","type":"string"},{"name":"adText","type":"string"}],"name":"placeImage","outputs":[{"name":"","type":"uint256"}],"payable":true,"type":"function"},{"constant":false,"inputs":[{"name":"x1","type":"uint8"},{"name":"y1","type":"uint8"},{"name":"x2","type":"uint8"},{"name":"y2","type":"uint8"}],"name":"buyBlocks","outputs":[{"name":"","type":"uint256"}],"payable":true,"type":"function"},{"constant":false,"inputs":[{"name":"refund","type":"bool"}],"name":"admin_refundInvestments","outputs":[],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"userAddress","type":"address"}],"name":"getUserInfo","outputs":[{"name":"referal","type":"address"},{"name":"handshakes","type":"uint8"},{"name":"balance","type":"uint256"},{"name":"activationTime","type":"uint32"},{"name":"banned","type":"bool"},{"name":"userID","type":"uint256"},{"name":"refunded","type":"bool"},{"name":"investments","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"stopped","type":"bool"}],"name":"admin_pauseContract","outputs":[],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"userID","type":"uint256"}],"name":"getUserAddressByID","outputs":[{"name":"userAddress","type":"address"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"getStateInfo","outputs":[{"name":"_numUsers","type":"uint256"},{"name":"_blocksSold","type":"uint16"},{"name":"_totalWeiInvested","type":"uint256"},{"name":"_numImages","type":"uint256"},{"name":"_setting_imagePlacementPriceInWei","type":"uint256"},{"name":"_numNewStatus","type":"uint256"},{"name":"_setting_delay","type":"uint32"}],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"withdrawAll","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"referal","type":"address"}],"name":"signIn","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"imageID","type":"uint256"}],"name":"getImageInfo","outputs":[{"name":"x1","type":"uint8"},{"name":"y1","type":"uint8"},{"name":"x2","type":"uint8"},{"name":"y2","type":"uint8"},{"name":"imageSourceUrl","type":"string"},{"name":"adUrl","type":"string"},{"name":"adText","type":"string"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"charityBalance","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"charityAddress","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"newDelayInSeconds","type":"uint32"}],"name":"admin_setDelay","outputs":[],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"_currentLevel","type":"uint256"},{"name":"_setting_delay","type":"uint256"}],"name":"getActivationTime","outputs":[{"name":"","type":"uint32"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"price","type":"uint256"}],"name":"admin_setImagePlacementPriceInWei","outputs":[],"payable":false,"type":"function"},{"inputs":[],"type":"constructor"},{"payable":false,"type":"fallback"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"newUser","type":"address"},{"indexed":false,"name":"invitedBy","type":"address"},{"indexed":false,"name":"activationTime","type":"uint32"}],"name":"NewUser","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"x1","type":"uint8"},{"indexed":false,"name":"y1","type":"uint8"},{"indexed":false,"name":"x2","type":"uint8"},{"indexed":false,"name":"y2","type":"uint8"},{"indexed":false,"name":"price","type":"uint256"}],"name":"NewAreaStatus","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"x1","type":"uint8"},{"indexed":false,"name":"y1","type":"uint8"},{"indexed":false,"name":"x2","type":"uint8"},{"indexed":false,"name":"y2","type":"uint8"},{"indexed":false,"name":"imageSourceUrl","type":"string"},{"indexed":false,"name":"adUrl","type":"string"},{"indexed":false,"name":"adText","type":"string"}],"name":"NewImage","type":"event"}]

- copy-paste contract name: 

.. code-block:: none

	My Million Ether

.. image:: /img/powered_by_ethereum.png 

- click ok

You now should be able to see My Million Ether contract in Contracts section.


**2. Sign in using a referral link (address)**

- From your web browser copy your referral's address and paste it into referral field (make sure there are no whitespaces).

.. image:: /img/powered_by_ethereum.png 

.. note::

	Alternatively your referral's address is everything after slash: themillionetherhomepage.com/**0x5dcd0da5e8506.........fe0c1d4f60a6c724918**

- Go to Contracts -> My Million Ether -> Write to contract -> Select function -> Sign In.

.. image:: /img/powered_by_ethereum.png 

- Click Execute and confirm transaction.

.. image:: /img/powered_by_ethereum.png 

.. note::

	The only ether you pay here is the gas price (Ethereum blockchain commission).

.. note::

	Your referral link is themillionetherhomepage.com/ + your public ethereum address. You can compose it yourself, but it is activated through sign in procedure only. 

.. note::

	If you receive **“It seems this transaction will fail, it may consume all the gas you send”** than check your referral's activation time. Go to Contracts -> My Million Ether -> Read from contract -> Get User Info. Copy-paste your referral's link and check the activation time. If the referral is not active yet, just wait for the :ref:`activation time<activation>` and try again.

Now you can share your link and start earning ether!



*************
Invite people
*************


**1. Sign in if you haven't yet** - :ref:`Sign in <sign-in>` 


**2. Copy your personal link.**

- Go to Contracts -> My Million Ether -> Read from contract -> Get my info. 

.. image:: /img/powered_by_ethereum.png 

.. note::

	Keep your activation time in my mind. You can start sharing your link but a person who tries to sign in with it will have to wait until your account activates. To check your activation time go to Contracts -> My Million Ether -> Read from contract -> Get my info -> Activation time. :ref:`More on activation time.<activation>`

Now you can use this link to invite other people to participate. Share this link on a blogpost, social networks or send it by email to your friends.


********************
Withdraw your reward
********************

**1. Check your balance**

- Go to Contracts -> My Million Ether -> Read from contract ->  Get my info.

.. image:: /img/powered_by_ethereum.png 


**2. Withdraw**

- Go to Contracts -> My Million Ether -> WRITE TO CONTRACT -> Select function -> Withdraw All

.. image:: /img/powered_by_ethereum.png 

- Click Execute and confirm transaction. 

In a couple of minutes (depending on block mining speed) your should be able to see your funds in your wallet. 