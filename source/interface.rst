.. _interface:

################################
Interact with the smart contract
################################

.. _sign-in:



**Requirements:**

If you don't have an Ethereum address yet, `go get one <http://ethereum.stackexchange.com/a/2071/2919>`_ and load it with some ETH.

**1. Start watching the MillionEther smart contract.**

- In EthereumWallet go to Contracts, scroll down and click Watch contract button.

.. image:: /img/watch_contract.png

- copy-paste the contract address:

.. code-block:: none

	0x15dbdB25f870f21eaf9105e68e249E0426DaE916 todo

- copy-paste the contract JSON INTERFACE:

.. code-block:: json

	[{"constant":false,"inputs":[{"name":"newDelayInSeconds","type":"uint32"},{"name":"newCharityAddress","type":"address"},{"name":"newImagePlacementPriceInWei","type":"uint256"}],"name":"adminContractSettings","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"emergencyRefund","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"},{"name":"priceForEachBlockInWei","type":"uint256"}],"name":"sellBlocks","outputs":[{"name":"","type":"bool"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"}],"name":"getAreaPrice","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"x","type":"uint8"},{"name":"y","type":"uint8"}],"name":"getBlockInfo","outputs":[{"name":"landlord","type":"address"},{"name":"imageID","type":"uint256"},{"name":"sellPrice","type":"uint256"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"},{"name":"imageSourceUrl","type":"string"},{"name":"adUrl","type":"string"},{"name":"adText","type":"string"}],"name":"placeImage","outputs":[{"name":"","type":"uint256"}],"payable":true,"type":"function"},{"constant":false,"inputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"}],"name":"buyBlocks","outputs":[{"name":"","type":"uint256"}],"payable":true,"type":"function"},{"constant":true,"inputs":[{"name":"userAddress","type":"address"}],"name":"getUserInfo","outputs":[{"name":"referal","type":"address"},{"name":"handshakes","type":"uint8"},{"name":"balance","type":"uint256"},{"name":"activationTime","type":"uint32"},{"name":"banned","type":"bool"},{"name":"userID","type":"uint256"},{"name":"refunded","type":"bool"},{"name":"investments","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"userID","type":"uint256"}],"name":"getUserAddressByID","outputs":[{"name":"userAddress","type":"address"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"getMyInfo","outputs":[{"name":"balance","type":"uint256"},{"name":"activationTime","type":"uint32"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"getStateInfo","outputs":[{"name":"_numUsers","type":"uint256"},{"name":"_blocksSold","type":"uint16"},{"name":"_totalWeiInvested","type":"uint256"},{"name":"_numImages","type":"uint256"},{"name":"_setting_imagePlacementPriceInWei","type":"uint256"},{"name":"_numNewStatus","type":"uint256"},{"name":"_setting_delay","type":"uint32"}],"payable":false,"type":"function"},{"constant":false,"inputs":[],"name":"withdrawAll","outputs":[],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"referal","type":"address"}],"name":"signIn","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[{"name":"imageID","type":"uint256"}],"name":"getImageInfo","outputs":[{"name":"fromX","type":"uint8"},{"name":"fromY","type":"uint8"},{"name":"toX","type":"uint8"},{"name":"toY","type":"uint8"},{"name":"imageSourceUrl","type":"string"},{"name":"adUrl","type":"string"},{"name":"adText","type":"string"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"charityBalance","outputs":[{"name":"","type":"uint256"}],"payable":false,"type":"function"},{"constant":true,"inputs":[],"name":"charityAddress","outputs":[{"name":"","type":"address"}],"payable":false,"type":"function"},{"constant":false,"inputs":[{"name":"violator","type":"address"},{"name":"banViolator","type":"bool"},{"name":"pauseContract","type":"bool"},{"name":"refundInvestments","type":"bool"}],"name":"adminContractSecurity","outputs":[],"payable":false,"type":"function"},{"inputs":[],"payable":false,"type":"constructor"},{"payable":false,"type":"fallback"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"newUser","type":"address"},{"indexed":false,"name":"invitedBy","type":"address"},{"indexed":false,"name":"activationTime","type":"uint32"}],"name":"NewUser","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"fromX","type":"uint8"},{"indexed":false,"name":"fromY","type":"uint8"},{"indexed":false,"name":"toX","type":"uint8"},{"indexed":false,"name":"toY","type":"uint8"},{"indexed":false,"name":"price","type":"uint256"}],"name":"NewAreaStatus","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"ID","type":"uint256"},{"indexed":false,"name":"fromX","type":"uint8"},{"indexed":false,"name":"fromY","type":"uint8"},{"indexed":false,"name":"toX","type":"uint8"},{"indexed":false,"name":"toY","type":"uint8"},{"indexed":false,"name":"imageSourceUrl","type":"string"},{"indexed":false,"name":"adUrl","type":"string"},{"indexed":false,"name":"adText","type":"string"}],"name":"NewImage","type":"event"}]

- copy-paste contract name: 

.. code-block:: none

	My Million Ether

.. image:: /img/million_ether_contract.png 

- click ok

You now should be able to see My Million Ether contract in Contracts section.

**Next steps:**

- :ref:`Buy pixels <buy>`
