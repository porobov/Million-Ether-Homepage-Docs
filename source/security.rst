.. _security:

##########################
Security and upgradability 
##########################

The MillionEther contract incorporates necessary security features listed in the `official paper by ConsenSys <https://github.com/ConsenSys/smart-contract-best-practices/>`_, making it safe against known attacks. It has simple contract structure, safe external calls and thorough tests coverage.

Following general philosophy of the same document The MillionEther contract is prepared for unknown attacks by incorporating failsafe measures (escape paths). If something goes wrong admin is allowed to pause/unpause the contract.

Contract architecture is modular and upgradeable. 

More details to come soon. For now please see the `code comments <https://github.com/porobov/million-ether-homepage-2-contract/tree/master/contracts>`_.

