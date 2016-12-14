#########
PLACE ADS
#########

There are 3 steps:
1. Sign in (if you haven't yet).
2. Buy pixels.
3. Place an ad or ads within your pixels.

:ref:`Sign in <sign-in>` **if you haven't yet**

.. _buy:

**********
Buy pixels
**********

.. _coordinates:

**1. Decide with the coordinates you would like to buy.**

- Go to TheMillionEtherHomepage.com/[somereferral] in your web browser and hover your cursor over a block.

- Find block coordinates shown in square brackets.

.. image:: /img/browser_coordinates.png

.. note::

	Pixels are sold in 10x10 pixel blocks. As there are 1000x1000 pixels 100x100 blocks are available for purchase. Blocks are referenced by [x:y] coordinates starting from the left upper corner. The left upper corner block is [1:1], the right bottom corner block is [100:100].

**2. Check the price and availability of the selected pixels.**

- In EthereumWallet Go to Contracts -> My Million Ether -> Read from contract ->  Get area price
- type in block coordinates you would like to buy.

*From x, From y, To x, To y*
	Type “from block” and “to block” coordinates if you are buying several blocks. If you would like to buy just one block (10x10 pixels) type the same from and to coordinates (e.g. From x 1, From y 2, To x 1, To y  2). 

.. image:: /img/block_price.png

*In this example 4 blocks (20x20 pixels) in the left upper corner are bought. The price here is 4 ETH (Ethereum Wallet shows it in wei by default).*

.. note::

	The price is shown in wei (ether smallest denomination, use `unit converter <http://ether.fund/tool/converter>`_). If you see 0 price it means, that some or all of the blocks are already bought and owner didn't set the sell price (decided to keep it). 

**3. Send transaction**

- In EhtereumWallet go to Contracts -> My Million Ether -> WRITE TO CONTRACT -> Select function -> Buy Blocks.

- Type in the same coordinates and price as in the previous step, click Execute and confirm the transaction. Here unlike previous step we buy just 1 block with coordinates [19,19].

.. image:: /img/buy_blocks.png

.. note::

	If you receive “It seems this transaction will fail, it may consume all the gas you send” do not send the transaction. Check the availability and price again (previous step). Maybe someone has already bought the blocks you are trying to buy.

.. note::

	To see your info written to the blockchain wait a couple of seconds until your transaction is mined (approx. 15 seconds for the Ethereum blockchain as of 12.14.2016). Go to Contracts -> My Million Ether -> Read from contract ->  Get block info type your coordinates and make sure your address appears. 

Now you can place your ad (scroll down for instructions) or chose to :ref:`sell blocks <sell>` later.

*********
Place ads
*********

As the most parts of this project image storage is decentralized. It is currently too expensive to place images within the blockchain we use imgur.com for image hosting. It is free and easy to use. 

**1. Upload your image to imgur.com.**

- Go to imgur.com and drag and drop your image to the website or click New post.

.. note::

	Please upload images with width and height corresponding to the pixels you bought otherwise cropping will occur (e.g. if you bought blocks from [1:1] to [1:2], upload two 10x10 px images or one 10x20 px image).

- Hover over the image, right-click and select **Copy image location**. You need a direct link - the one which ends with .jpg or .png. 

.. image:: /img/imgur.jpg

- Go to Contracts -> My Million Ether -> WRITE TO CONTRACT -> Select function -> Place Image.

From x, From y, To x, To y
	type coordinates to place image to (place as many 10x10 px images as you can fit within your area). If you would like to place 10x10 pixels image type the same from and to coordinates (e.g. From x  1, From y  2, To x  1, To y  2).
Image source url
	paste your imgur image link from the previous step (Links from other hosting services will be stored in the blockchain, but will not appear at TheMillionEtherHomepage.com)
Ad url
	put your website address. Make sure to put a valid url. Internationalized domain names (chinese, russian, greek, etc.) are not supported. Make sure you are not advertising anything obscene - :ref:`Read our advertising policies <policies>`. 

Ad text
	put your 140 character ad text which will appear when somebody hovers over your ad. Use `Twitter <https://twitter.com/>`_ or `charactercountonline.com <http://www.charactercountonline.com/>`_ to measure the length (Longer ad text will be stored in the blockchain, but appear truncated at TheMillionEtherHomepage.com)
Send Ether
	leave 0

.. image:: /img/place_ads.jpg 

*In this example an ad occupying 4 blocks (20x20 pixels) is submitted.*	

- Click Execute and confirm transaction.

.. note::

	If you receive “It seems this transaction will fail, it may consume all the gas you send” do not send the transaction and check the coordinates. Go to Contracts -> My Million Ether -> Read from contract ->  Get block info type your coordinates and make sure your address appears.

.. note::

	To see your info written to the blockchain wait a couple of seconds until your transaction is mined (approx. 15 seconds for the Ethereum blockchain as of 11.17.2016). Go to Contracts -> My Million Ether -> Read from contract ->  Get block info type your coordinates and copy Image id. Go to  Contracts -> My Million Ether -> Read from contract ->  Get image info and paste your image id. 

In a couple of minutes your ad will appear at TheMillionEtherHomepage.com.