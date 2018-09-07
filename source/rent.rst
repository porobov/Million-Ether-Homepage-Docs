.. _rent:

###########
RENT PIXELS
###########

You can rent an area if the owner set the rent price and if there is no active rent.

.. _rent_price:

**1. Check rent status and get rent price**

.. note::

    If you are buying an area, you probably want no active rent. Otherwise you'll have to wait until rent expires to place your ads (you can still sell the area anytime).

- In :ref:`contract interface <interface>` select **areaRentPrice** function (in some wallets may appear under Read section or similar).

- Specify function parameters.

    *fromX, fromY, toX, toY:*
        :ref:`coordinates <coordinates>` you would like to rent or check rent status.
    *numberOfPeriods:*
        number of days you would like rent to last. To check the rent status when buying area, put 1 or any number above 0 here (max 90 days).

- Click **Read** (you are not paying any gas here). There are 3 possible outcomes:

    *Rent price is 0*
        the owner is not willing to rent it out. If this area is on sale you can buy it and place your ads immediately.
    *Function returns error (throws)*
        there are one or more blocks with active rent. These are not available for rent until rent expires. You can buy this area, but you'll have to wait until rent expires to place your ads (you'd probably wanna :ref:`cancel further rent deals <cancel_rent>`).
    *Rent price is more than 0*
        area is available for rent. **Copy the price and proceed to the next step.**

**2. Rent area**

- In :ref:`contract interface <interface>` select **rentArea** function (in some wallets may appear under Write section or similar).

- Specify the same function parameters as in the previous step

    fromX, fromY, toX, toY:
        :ref:`coordinates <coordinates>` you would like to rent.
    numberOfPeriods:
        number of days you would like rent to last (max 90 days).

- Select your wallet and click **Write**.

    *Amount to Send*
        Paste the price in wei obtained at the previous step
    *Gas Limit*
        Should be calculated automatically.

- Click **Generate transaction**, sign it, send it and wait until it is mined.

.. note::

    If you receive “It seems this transaction will fail, it may consume all the gas you send” or something similar do not send the transaction. Make sure you're typing in the right coordinates, rent period and rent price.

**Next steps:**

Now you rent an area of pixels. Next you can:

- :ref:`Place your ads <ads>`