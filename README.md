# Fabric_Implementation
This repository contains the necessary files that need to be added to certain Hyperledger Fabric directories to setup and run the Fabric for storing image data.

1) First, prerequisites for running Hyperledger Fabric must be downloaded. This can be done by carefully following the instructions found at https://hyperledger-fabric.readthedocs.io/en/release-2.2/prereqs.html
2) Next, Fabric samples, Binaries and Docker Images need to be downloaded. This can be done by carefully following the instructions found at https://hyperledger-fabric.readthedocs.io/en/release-2.2/install.html
3) Now, the test network is ready for deployment. Two key steps are to be followed here: 
  i) First, copy the imagestore folder from Fabric_Implementation/imagestore and paste it in fabric/fabric-samples/ directory of Hyperledger Fabric. 
  ii) Second, copy imagestore folder from Fabric_Implementation/chaincode/imagestore and paste it in fabric/fabric-samples/chaincode/ directory of Hyperledger Fabric.
4) Under fabric/fabric-samples/chaincode/imagestore/javascript run **$npm install**. Under fabric/fabric-samples/imagestore/javascript run **$npm install**
5) To install nodejs-SDK, run **$npm install fabric-network** and to install fabric-contract-api, run **$npm install -save fabric-contract-api**

After the above steps have been completed, go to fabric/fabric-samples/imagestore and run **$./startNetwork.sh javascript**. This will start the fabric network. 
Now, go to /imagestore/javascript and run **$node enrollAdmin.js** and **$node registerUser.js**
Finally, go to /javascript and run **$node finalserver.js**
