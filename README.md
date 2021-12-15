# Fabric_Implementation
This repository contains the necessary files that need to be added to certain Hyperledger Fabric directories to setup and run the Fabric for storing image data.

1) First, prerequisites for running Hyperledger Fabric must be downloaded. This can be done by carefully following the instructions found at https://hyperledger-fabric.readthedocs.io/en/release-2.2/prereqs.html
2) Next, Fabric samples, Binaries and Docker Images need to be downloaded. This can be done by carefully following the instructions found at https://hyperledger-fabric.readthedocs.io/en/release-2.2/install.html
3) Now, the test network is ready for deployment. Two key steps are to be followed here: 
  i) First, copy the imagestore folder from Fabric_Implementation/imagestore and paste it in fabric/fabric-samples/ directory of Hyperledger Fabric. 
  ii) Second, copy imagestore folder from Fabric_Implementation/chaincode/imagestore and paste it in fabric/fabric-samples/chaincode/ directory of Hyperledger Fabric.
4) Under fabric/fabric-samples/chaincode/ run \$npm install. Under fabric/fabric-samples/imagestore run \$npm install
