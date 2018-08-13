.. _sell:

###########
SELL PIXELS
###########

o
o
o
o
o
o

**UNDER DEVELOPEMENT**

o
o
o
o
o
o

**1. Sell area**

Sell pixels to anybody. Just set the price. Buying process for the buyers will look exactly the same as if they bought it at the initial sale. You get all the money (no fees).

- In :ref:`contract interface <interface>` select **sellArea** function (in some wallets may appear under Write section or similar). 

- Specify function parameters.

fromX, fromY, toX, toY:
	:ref:`coordinates <coordinates>` you would like to sell.
priceForEachBlockWei:
	price for each 10x10 pixel block in wei (`Ether unit converter <http://ether.fund/tool/converter>`_).

- Send transaction and wait until it is mined.

.. image:: /img/sell_blocks.jpg 

*e.g. If you would like to sell two blocks from [1:1] to [1:2] for 20 ETH total set the Price for each block in wei to 10000000000000000000 (which is 20/2 * 10^18)*

.. note::

    If you receive “It seems this transaction will fail, it may consume all the gas you send” or something similar do not send the transaction. Make sure you're typing in the right coordinates (:ref:`make sure the area belongs to you <area_ownership>`

**2. Make sure that the area is now on sale**

- In :ref:`contract interface <interface>` select **areaPrice** function (in some wallets may appear under Read section or similar).

- Specify the coordinates you would like to check.

- Check that the total price you see is the one you want. 

.. note::

    Remember that when selling area you specify price for each 10x10 pixels block. Here you get the total price for the whole area. The price is wei (`Ether unit converter <http://ether.fund/tool/converter>`_).

**3. Cancel sale**

Just set the sell price to zero:

- In :ref:`contract interface <interface>` select **sellArea** function (in some wallets may appear under Write section or similar). 

- Specify function parameters.

fromX, fromY, toX, toY:
    coordinates you would like to stop selling.
priceForEachBlockWei:
    set this price to 0.

- Send transaction and wait until it is mined.