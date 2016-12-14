===========
WHITE PAPER
===========

**TheMillionEtherHomepage.com** is a decentralized advertising platform based on the blockchain technology.

Main features
-------------

1. 1000х1000 pixels field. 
2. Pixels may be bought, sold or used to place ads. 
3. Income is decentralized and shared between referrals (and charity). 

Interaction with the platform is done through **MillionEther smart contract** sitting in the Ethereum blockchain. Which means there is no need to trust anybody as the contract code is open. TheMillionEtherHomepage.com is just the representation of what is happening in the smart contract.

`More on smart contracts <http://blockgeeks.com/guides/smart-contracts-the-blockchain-technology-that-will-replace-lawyers/>`_

6 handshakes 
------------
The most important feature of the platform is that income is decentralized and goes entirely to referrals (and charity).

It is invitation only. The referral link is needed to sign in and to buy pixels (place ads). Once you sign in you get your own referral link and may start sharing it. When anybody buys pixels the chain of referrals (handshakes) which led to the buyer gets all the money. The referral closest to the buyer (1 handshake) gets 50% of the purchase price, next one (2 handshakes) gets 25%, next (3 handshakes) 12,5% and so on.

.. image:: /img/net.jpg

**Example:**

*Bob signs in and receives his personal link  themillionetherhomepage.com/0xf39d..0b1cf78. He writes a blog post where he shares his link. Alice reads the Bob's post and uses his link to sign in to the platform. Alice gets her personal link and sends it to Mike. Mike signs in and decides that it's a perfect chance to advertise his product. Mike buys 100 pixels for 100 ETH. Alice gets 50 ETH, Bob gets 25 ETH. Bob gets another 12,5 ETH as July uses his link to sign in, invites Sam and Sam buys 50 pixels for 50 ETH.*

**Payout chain is maximum 6 levels deep (6 handshakes).**

If the chain reaches 6 handshakes length the last referral on the chain gets 1,5625% of the purchase price and remaining 1,5625% is donated to charity. 

.. image:: /img/long-chain.jpg

**A chain shorter than 6 handshakes ends with Administrator's account.** 

Administrator gets payed by the same principle as any other referral. This is the only income of the project, which is needed to support off chain infrastructure (maintaining website and pushing data to it require some USD).

.. image:: /img/short-chain.jpg

The shorter the chain the more money you get and the more money is sent to charity. So please find the most effective routes.

:ref:`How to sign <sign-in>`

Buying pixels
-------------
Pixels are available in 10x10 pixel blocks. Once you buy a block (or blocks), you may put an ad (image with a link and description) within that block (or blocks) or decide to sell it later.

:ref:`How to buy pixels and place ads<buy>`

Selling pixels (Investment  opportunity)
----------------------------------------
The initial purchase price doubles with every 100 000 pixels sold. If you buy pixels early you can have significant profit selling them later (no fees here). All you have to do is set your price.

:ref:`How to sell pixels <sell>`

Placing ads
-----------
An ad is an image with description and a link to your website. The minimum image size is 10x10 pixels. You can place as many images as you can fit within owned area. You can also replace images unlimited number of times. Description is 140 characters long. 

:ref:`How to buy pixels and place ads<buy>`

*The fee for placing ads is currently set to 0. Please note that the smart contract administrator is allowed to set this fee if needed in the future (as it requires off chain computations to push images to the website). For details see* :ref:`Admin privileges <admin>`

*Please read the rules for images allowed on the platform:* :ref:`Advertising policies <policies>`

Pixel price
-----------
The pixel price doubles with every 100 000 pixels sold. This allows investment opportunities and rewards early birds. 

.. image:: /img/pixel-price.jpg

.. _activation:

User activation time
--------------------
With every handshake far from the Root (Admin) user activation time increases by 2 being 1, 2, 4, 8, 16 hours and so on. We encourage shorter (and faster) chains to increase charity donations, project support and referrals incomes (by preventing  one user with many accounts filling up the whole referral chain and get all the  income). 

We believe it also brings us closer to our side goal - the small world experiment on blockchain. `More on the small world experiment <https://en.wikipedia.org/wiki/Small-world_experiment/>`_

Links
-----
`Million Ether contract at Etherscan.io <https://etherscan.io/address/0x15dbdB25f870f21eaf9105e68e249E0426DaE916/>`_

`Million Ether contract at Github <https://github.com/porobov/MillionEtherHomepage/>`_