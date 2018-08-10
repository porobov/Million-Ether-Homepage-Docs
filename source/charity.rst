.. _charity:

#######
Charity
#######

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

**Charity deductions**

80% of initial sale income automatically goes to charity. Charity is deducted through transferFundsToAdminAndCharity_ function.

Charity funds are stored in a special balance inside the contract. Current charity balance can be monitored the same way you :ref:`monitor your own balance. <check_bal>`

Use this charity vault address as input for the balance function:  "**0x616c6C20796F75206e656564206973206C6f7665**" (charityVault_ variable). 

.. note::

    The address string is **"all you need is love"** in hex format - insures nobody has access to it.

**Funds distribution**

The distribution of funds among charitable organizations is **done manually**. 

Owner of the contract calls adminTransferCharity_ function and specifies an amount and a receiver address. The amount is transferred from vault balance to receiver's balance. On transfer LogCharityTransfer_ event is fired and charityPayed_ public variable is incremented by the amount transferred. Receivers then need to withdraw their balance.

A receiver is either an address of one of the :ref:`preferred charitable organizations<charities>` or a special single address **owned by the contract owner** being used exclusively for funds forwarding (`forwarding address`_).

**Why use manual funds distribution?**

Because other options would require too much code. Which is more bugs and more constraints. But we want flexibility and security. We want to transfer any amount to any charity at anytime. So a little bit of good old centralization won't harm.

Instead of making it trustless let us build trust. In other words just watch funds being **continuously sent to charities** and **trust** that this will continue to happen. 

This is where charity earned by the previous version of TheMillionEtherHomepage.com went (to giveth.io). todo links

**How to control charity distribution?**

The easiest way to control funds distribution is to check this `Google Spreadsheet file`_. It lists all charity operations and summarizes them. First check that totals match and then randomly find several transaction on block explorer and check them too.

For a more thorough examination:

- Check 0x616c6C20796F75206e656564206973206C6f7665 address balance to see how much of the charity funds is stored in the contract. 
- Check charityPayed public variable to see how much charity is payed out.
- Check LogCharityTransfer_ events to see where the charity funds go.
- If any of the funds were forwarded through the `forwarding address`_ see where the charity funds go through Etherscan (the address is used for charity transactions only).

.. _charities:

**Preferred charity organizations**

Projects addressing life and death problems are preferred (no software, art, info leaks donations, etc). The list is maintained in this repo_ (pull requests are welcome).

.. note::

    Most of the charitable organizations in the list are centralized. There is no way to control further usage of funds.









.. _charityVault: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L36
.. _transferFundsToAdminAndCharity: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L227
.. _adminTransferCharity: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L168
.. _LogCharityTransfer: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L48
.. _charityPayed: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L37
.. _forwarding address: https://todo
.. _Google Spreadsheet file: https://todo2
.. _repo: https://github.com/porobov/charities-accepting-ether