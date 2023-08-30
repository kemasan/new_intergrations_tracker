# new_intergrations_tracker


This repository contains the documentation for the tracking process of token holders, which involves several steps to identify and categorize different types of addresses using APIs and data sources. The goal of this process is to find new protocols that integrate stAssets, maintain an up-to-date and organized list of token holders' addresses for analysis and reporting purposes.

Steps
Step 1: get token_address via API
In this initial step, we retrieve a list of token holders' addresses by interfacing with an API.

Step 2: filter for the contract addresses
Once we have obtained the list of token holder addresses, we proceed to check each address to determine if it is a contract address.

Step 3: filter for the already-known contract addresses
We combine the list of verified contract addresses, obtained from the previous step, with the list of token holders' addresses that we already have from the DUNE data source. This merging process allows us to associate names with contract addresses.

Step 4: tag Unknown Addresses
Addresses that are not present in our existing list of token holders are classified as unknown. We add these addresses to the list of holders' addresses with the tag "TBD" (To Be Determined) for further identification process.

Step 5: verify Unknown New Token Addresses
Within this step, we verify whether the unknown new addresses are indeed token addresses. If they are identified as valid token addresses, we add them to the list of LSTs with the tag "TBD." for further identification process.

Contribution
We welcome contributions and suggestions to enhance the accuracy and efficiency of our token holder tracking process. If you have any improvements or ideas, please feel free to create pull requests or open issues.



