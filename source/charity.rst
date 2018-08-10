.. _charity:

#######
Charity
#######

**Charity deductions**

80% of initial sale income automatically goes to charity. Charity is deducted through transferFundsToAdminAndCharity_ function.

Charity funds are stored in a special balance inside the contract. Current balance can be monitored the same way you :ref:`monitor your own balance. <check_bal>`

Use this charity vault address as input for the balance function:  "0x616c6C20796F75206e656564206973206C6f7665" (charityVault_ variable). 

.. note::

    The address string is **"all you need is love"** in hex format - insures nobody has access to it.

**Distribution**

The distribution of funds among charities is done manually. 

Owner of the contract calls adminTransferCharity_ function and specifies an amount and a receiver address. On transfer LogCharityTransfer_ event is fired and charityPayed_ public variable is incremented. 

A receiver is either an address of one of the preferred_charity_organizations_ or a special single address **owned by the contract owner** for further forwarding.

**Why use manual funds distribution?**

So as you can see the charity is distributed manually. This allows maximum flexibility. 

**Why use a forwarding address?** 

To receive funds a charity will need to call withdraw function. Meaning they need to make a minimal audit of the contract. Forwarding_address_ will allow more flexibility.

**How can I trust**
Immutability vs flexibility. 
More secure (less code), more flexible (some will not accept direct send, some will not withdraw)

**How to control charity distribution?**

- Check 0x616c6C20796F75206e656564206973206C6f7665 address balance to see how much of the charity funds is stored in the contract. 
- Check charityPayed public variable to see how much charity is payed out.
- Check LogCharityTransfer_ events to see where the charity funds go.
- If any of the funds were forwarded through the forwarding_address_ see where the charity funds go through Etherscan. 

.. _preferred_charity_organizations:

**Preferred charity organizations**

Projects addressing life and death problems are preferred (no software, art, info leaks donations, etc). The list is maintained in this repo_ (pull requests are welcome).










.. _charityVault: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L36
.. _transferFundsToAdminAndCharity: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L227
.. _adminTransferCharity: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L168
.. _LogCharityTransfer: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L48
.. _charityPayed: https://github.com/porobov/million-ether-homepage-2-contract/blob/f72ca9526ad25934bff36e7c7691e84abdd7a6ef/contracts/Market.sol#L37
.. _forwarding_address: https://todo
.. _repo: https://github.com/porobov/charities-accepting-ether