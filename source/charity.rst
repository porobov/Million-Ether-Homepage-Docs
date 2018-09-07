.. _charity:

#######
Charity
#######

.. _charities:

**Preferred charity organizations**

Projects addressing life and death problems are preferred (no software, art, info leaks donations, etc). The list of charities is maintained in this repo_ (pull requests are welcome).

**Charity deductions**

80% of initial sale income automatically goes to charity (see transferFundsToAdminAndCharity_ function).

Charity funds are stored at special balance inside the contract. Current charity balance can be monitored the same way you :ref:`monitor your own balance. <check_bal>`

Charity vault address is:  "**0x616c6C20796F75206e656564206973206C6f7665**" (hardcoded in charityVault_ variable). 

.. note::

    Charity address string is **"all you need is love"** in hex format - insures nobody has access to it.

**Funds distribution**

The distribution of funds among charitable organizations is **done manually** (though totally transparently). 

Owner of the contract calls adminTransferCharity_ function and specifies an amount and a receiver address. The amount is transferred from vault balance to receiver's balance. On transfer LogCharityTransfer_ event is fired and charityPayed_ public variable is incremented by the amount transferred. Receivers then need to withdraw their balance.

A receiver is either an address of one of the :ref:`preferred charitable organizations<charities>` or a special single address **owned by the contract owner** being used exclusively for funds forwarding (`forwarding address`_).

**Why use manual funds distribution?**

Simple answer - it is simpler. Other options would require a lot more coding, which is more bugs and more constraints. But we want flexibility and security. We want to transfer any amount to any charity at anytime. So a little bit of good old centralization won't harm.

Instead of making it trustless let us build trust. In other words just watch funds being **continuously sent to charities** and **trust** that this will continue to happen in the future. 

**How to control charity distribution?**

The easiest way to control funds distribution is to check this `Google Spreadsheet file`_. It lists all charity operations and summarizes them. First check that totals match and then randomly find several transaction on block explorer and check them too.

For a more thorough examination:

- Check 0x616c6C20796F75206e656564206973206C6f7665 address balance to see how much of the charity funds is stored in the contract. 
- Check charityPayed public variable to see how much charity is payed out.
- Check LogCharityTransfer_ events to see where the charity funds go.
- If any of the funds were forwarded through the `forwarding address`_ see where the charity funds go through Etherscan (the address is used for charity transactions only).

.. note::

    Most of the charitable organizations in the list are centralized. There is no way to control further usage of funds.


.. _charityVault: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L36
.. _transferFundsToAdminAndCharity: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L227
.. _adminTransferCharity: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L168
.. _LogCharityTransfer: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L48
.. _charityPayed: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L37
.. _forwarding address: https://etherscan.io/address/0xed4799B6fc0d69571e5c26676b88e15588ff1bFf
.. _Google Spreadsheet file: https://docs.google.com/spreadsheets/d/e/2PACX-1vSSym40-E4ZJvBWcQ87C57MeCz5FfjoHnNxG9FzjjMs5wOMrxFeLesFpXJrrf1jneWV05xubp12Ok_6/pubhtml
.. _repo: https://github.com/porobov/charities-accepting-ether