.. _old:

#############
Older version
#############

The previous version of TheMillionEtherHomepage smart contract is at this address_. Documentation is available by choosing million-ether-homepage-1 version of this docs. Source files are available at Github_.

The main reason to terminate the previous version is that it is priced in Ether. Starting price was 1 ETH. It was launched when Ethereum price was around $8. Hardly anyone would buy a 10x10 pixel block for 1 ETH nowadays (unless ETHUSD drops significantly - let's hope it won't).

**Importing blocks**

Sales and ads were imported to the new version. All block ownership was imported prior to launch through adminImportOldMEBlock_ function. Ads ids were incremented accordingly as well. Whether new sales occur they will not be imported to the new version.

**Charity**

Previous version is a charity project as well. All earned charity funds were donated to Giveth.io and can be tracked through this `Google Spreadsheet file`_.

**Current state**

The smart contract still accepts transactions. No more sales though if they occur will be imported to the new version. 

There is currently no representation of the smart contract state in the web. TheMillionEtherHomepage.com now represents only new version.


.. _Github: https://github.com/porobov/MillionEtherHomepage
.. _address: https://etherscan.io/address/0x15dbdB25f870f21eaf9105e68e249E0426DaE916
.. _adminImportOldMEBlock: https://github.com/porobov/million-ether-homepage-2-contract/blob/bbff20979b1f511e27458563a9ca82f038d5103e/contracts/MEH.sol#L275
.. _Google Spreadsheet file: https://docs.google.com/spreadsheets/d/e/2PACX-1vSSym40-E4ZJvBWcQ87C57MeCz5FfjoHnNxG9FzjjMs5wOMrxFeLesFpXJrrf1jneWV05xubp12Ok_6/pubhtml