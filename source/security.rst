.. _security:

########
Security
########

The MillionEther contract incorporates necessary security features listed in the `official paper by ConsenSys <https://github.com/ConsenSys/smart-contract-best-practices/>`_, making it safe against known attacks, including Recursive call attack (DAO ATTACK). It has simple contract structure, no external calls and 100% tests coverage.
 
Following general philosophy of the `same document <https://github.com/ConsenSys/smart-contract-best-practices/>`_ The MillionEther contract is prepared for unknown attacks by incorporating failsafe measures (escape paths). If something goes wrong admin is allowed to pause/resume the contract, freeze/unfreeze users, issue refunds. 

:ref:`Administrator priveleges <admin>`