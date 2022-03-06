# Basic Sample Project
You need hardhat

run
>> npm install --save-dev hardhat

run
>> npx hardhat


Now
Deploy to polygon

Go to the hardhat.config file and uncomment out the following

//mumbai: {
//   url: "https://rpc-mumbai.maticvigil.com/",
// accounts: [process.env.pk]
//},

Run
>> npx hardhat node


Setup metamask * get your pk
In another window
>> export pk="your-private-key"

Setup mumbai testnet on metamask
Go to the bottom of this page and click on setup mumbai
https://mumbai.polygonscan.com/

Send yourself some fake MATIC with the faucet
https://faucet.polygon.technology/

In the project file ensure that .env.local in root, is set to "local" on both items
ENVIRONMENT="local"
NEXT_PUBLIC_ENVIRONMENT="local"

Go back to the hardhat.config file and now uncomment out the mumbai parts

Run
>> npx hardhat run scripts/deploy.js --network mumbai

Go back to .env.local and set both items to "testnet"

Run
>>npm run dev
