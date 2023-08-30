# new_intergrations_tracker


This repository contains the documentation for the tracking process of token holders, which involves several steps to identify and categorize different types of addresses using APIs and data sources. The goal of this process is to find new protocols that integrate stAssets, and maintain an up-to-date and organized list of token holders' addresses for analysis and reporting purposes.


Requirements:

    python, pip, jupyter notebook (any other working environment)

Instruction:

    create and activate a virtualenv

    open notebook in browser

Working notebook

To extract token holders' addresses from Ethplorer needs to use its API (see for Ethplorer API --> getTopTokenHolders) and Infura to simplify access to web3 infrastructure

    import the required libraries and packages

    create a function to holders' addresses filter for contract addresses: def is_contract(vaddr)

    create a function to parse row data: def parse_holders_contracts(df)

    create a tokens data frame: pd.DataFrame(pd.read_csv('eth_LSDs.csv'))

    create a holders' data frame (already known addresses): pd.DataFrame(pd.read_csv('eth_holders.csv'))

    create a 'for' loop to get holders of each token from the tokens data frame, merge all holders' date, then compare with 
    known holders' addresses, tag unknown addresses as 'TBD', save .csv file: for token_address in lsd.minted_token_address...
      
    create a 'for' loop to check if unknown addresses are token addresses, and if they are token addresses, add 
    them to the list of LSTs with the tag 'TBD'


Contribution
We welcome contributions and suggestions to enhance the accuracy and efficiency of our token holder tracking process. If you have any improvements or ideas, please feel free to create pull requests or open issues.



