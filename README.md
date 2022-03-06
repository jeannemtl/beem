# Basic Sample Project

Deploy to polygon

Setup metamask * get your pk

Run
>> export pk="your-private-key"

Setup mumbai testnet on metamask
Go to the bottom of this page and click on setup mumbai
https://mumbai.polygonscan.com/

Send yourself some fake MATIC with the faucet
https://faucet.polygon.technology/

In the project file ensure that .env.local is set to "local" on both items

Run
>> npx hardhat run scripts/deploy.js --network mumbai

Go back to .env.local and set both items to "testnet"

Run
>>npm run dev
