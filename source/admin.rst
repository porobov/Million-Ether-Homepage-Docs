.. _admin:

########################
Administrator priveleges
########################

**Moderating ads**

If somebody violates platform's :ref:`advertising policies <policies>` administrator is allowed to replace/delete user's ad, freeze/unfreeze user, forcibly mark user's pixels for sale (the user will still be able to withdraw rewards). 

**Security**

If something unexpected happens with the blockchain or contract itself administrator is allowed to Pause/Resume contract and Issue refunds. See :ref:`Security <security>`.

**Contract settings**

User activation time 
	is set to 1 hour by default and increases with every “handshake” far from the Root(Administrator). See :ref:`User activation time <activation>` for details. Admin is allowed to set arbitrary activation time. 

Charity address 
	is empty by default. Until a charity address is set all donations accumulate within the contract. After a charity address is set it receives charity funds. Admin is allowed to set charity address. The voting for the address will be held off chain as it is simpler than implementing voting logic within the contract. Admin has too little incentive to cheat on that.

Image placement price
    is set to 0 by default. Please note that the smart contract owner is allowed to set this fee if needed in the future (as it requires fiat to host the website).


More detalis to come soon. For now please see the code comments.
