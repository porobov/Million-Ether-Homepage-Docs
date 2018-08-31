.. _withdraw:

############
WITHDRAW ETH
############

Income from sold and rented pixels goes to your balance within the contract.

Every excess funds you send to buy or rent functions are returned to your balance as well. 

.. _check_bal:

**1. Check your balance**

- In :ref:`contract interface <interface>` select **balances** function (in some wallets may appear under Read section or similar).
- Paste your address.
- Click **Read** (you are not paying any gas here).

Your balance will be displayed in wei (`Ether unit converter <http://ether.fund/tool/converter>`_). 

**2. Withdraw**

- In :ref:`contract interface <interface>` select **withdraw** function (in some wallets may appear under Write section or similar).
- Select your wallet and click **Write**.

    *Amount to Send*
        0 (do not send any ether)
    *Gas Limit*
        Should be calculated automatically.

.. image:: /img/withdraw.png 

After a while (depending on block mining speed) you should be able to see your funds in your wallet.
