# TypeBeat NFT Marketplace
For ETHOnline Hackathon
[![Add to Homescreen](https://img.shields.io/badge/Skynet-Add%20To%20Homescreen-00c65e?logo=skynet&labelColor=0d0d0d)](https://homescreen.hns.siasky.net/#/skylink/[CADTtiQfTQnICfhmWIReLRAG4WOm2G95RY3cZi92uKDe_w])
## Steps to run this application

Clone this repo

Install the project
``` 
yarn add all
```

## Compile the contract

To compile the contract, just go

```
truffle compile --network mumbai
```

## Testing Contract

In a new terminal start a local blockchain using
```
truffle develop
```

To test:
```
truffle test --network develop
```

## Configuring Deployment

Now to deploy the NFT contract on the Polygon Mumbai Testnet.

Next, set up a Mumbai Testnet provider. You can get one from https://alchemyapi.io.
Next, configure network providers in *truffle-config.js*.
You must add your own *12 word account seed phrase* by creating a **.secret** file in the base folder.
and your *api key* by creating a **.apikey** file in the base folder.
<br>

## Deploy Contract

If everything is configured properly, you can now deploy. In your terminal, run the deploy command

```
truffle migrate --reset --network mumbai
```

## Important

After testing please remove the **.json** files from *src/contracts/* before each newer contract deployment.