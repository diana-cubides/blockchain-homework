#Blockchain Initizaliation


> ***Create Accounts***

While in the Blockchain Folder, using Gitbash create the account(s) with geth (use password). Use the node name as desired. 

./geth --datadir node6 account new

This will trigger the creation of a folder with the node name in the main folder


> ***Run Puppeth - Create Network***

 Run ./puppeth command which will prompt access to Ethereum provate network manager. 

 Here, a new network will be created. The name of this network will be the same one to set up MyCrypto app. 

 In these steps, the blockchain is created and atributes are given to it, such as what type of algorithm it will use, pre-fund features, among others. 

 As a result of this line of commands, json extension files will be created, which later will be used to open the digital wallet.

> ***Initialize nodes***

Run command ./geth --datadir node5 init unithw.json to initialize nodes. 

Then run command ./geth --datadir node5 --unlock "0xe5b93AAC5C9D18417Ddc0C4884C43A74e6709E53" --mine --rpc --allow-insecure-unlock to unlock and get relevant information such as the first enode, which will be used to unlock the second one. By running this forst command, the first block is ready to be mined. 

In a different instance of Git Bash, fire up second node, using the e node from the first one

> ***Transfering to MyCrypto***

In order to be able to transact with the 2 nodes created, in My Crypto we need to create a network with the same name as we used. After providing authetication necessary it is possible to link the accounst fo the nodes created to the wallet. 

Once those are loaded, we can transact among those 2 accounts and the transaction will be mined and confirmed. 
