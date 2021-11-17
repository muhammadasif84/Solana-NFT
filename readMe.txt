SOLANA
DOCS link => https://docs.metaplex.com
Video Link => https://www.youtube.com/watch?v=35RO0lAEIxE&t=156s

IN SOLANA WE USE SOLSCAN OR ETHERSCAN AS WELL FOR CHECK TRANSACTIONS.
WE USE PHANTON WALLET FOR SOLANA(MAINNET, DEVNET, TESTNET).
DOWNLOAD ZIP SOURCE FILE FROM HASHLIPS/hashlips_art_engine for NFT (GitHub Repo).
DOWNLOAD ZIP SOURCE FILE FROM metaplex-foundation/metaplex(GitHub Repo), METAPLEX MASTER.
DOWNLOAD ZIP SOURCE FILE FROM exiled-apes/candy-machine-mint(GitHub Repo).

CODING
****HASHLIPS/hashlips_art_engine****
UNZIP AND OPEN  HASHLIPS/hashlips_art_engine FILE IN VSCODE AND RUN npm install (under hashlips_art_engine folder).
OPEN config.js file within src folder and change network from ETH to Sol and change SolanametaData.
RUN npm run generate , this command will generate BUILD folder.
BUILD folder consists of images and json files of images, in solana serial start from 0123.
Make a new folder and named it "assests" drag the images and json file from BUILD folder tp assests folder, 
leave the _metadata.json file.
DRAG the assests folder to METAPLEX MASTER folder.

****METAPLEX MASTER****
OPEN METAPLES MASTER folder in VSCODE.
WE need to install SOLANA CLI.
**Prerequisites**
git Installation (ZIP FILES)
node Installation (INSTALLED)
yarn Installation (INSTALLED "npm install yarn" OR "npm")
ts-node Installation 
Install the Solana Tool Suite CLI, where we can generates nft's.
INSTALLED as a "administer cmd".
Download Prebuilt Binaries.
Download the binaries by navigating to https://github.com/solana-labs/solana/releases/latest,
download solana-release-x86_64-pc-windows-msvc.tar.bz2,
then extract the archive using WinZip(https://www.ezyzip.com/) or similar.
INSTALLED NETWORK which is DEVNET(phonton wallet) "solana config set --url https://api.devnet.solana.com".
(1)CREATE devnet wallet (for testing) solana-keygen new --outfile ~/.config/solana/devnet-pluton.json.
SAVEd S in info file.
ADD / CONNECT new phonton wallet test1,
import PK from ~/.config/solana/devnet-pluton,
paste it in test1.(see 1).
(2)RUN keypair command "solana-keygen new -o" and add (see1) ~/.config/solana/devnet-pluton.json,
complete command to be run "solana-keygen new -o ~/.config/solana/devnet-pluton",
executed file Config File: C:\Users\SEO\.config\solana\cli\config.yml
RPC URL: https://api.devnet.solana.com 
WebSocket URL: wss://api.devnet.solana.com/ (computed)
Keypair Path: ~/.config/solana/devnet-pluton
Commitment: confirmed.
CHECK your account balance for test1 account run "solana balance".
GET some fake solana for test run "solana airdrop 3(any number)" it will give you 3 fake solana,
some of SOLANA commands solana balance, solana address, solana airdrop 5 many more.
CD to js file like "cd js".
RUN "yarn install".
RUN "yarn bootstrap".
CD to main root folder like "cd ..".
CREATING frontend dapp and link it to devnet(test net) with following commands,
npx ts-node js/packages/cli/src/candy-machine-cli.ts upload ./assets --env devnet --keypair (PATH),
this command will create a .cache folder

npx ts-node js/packages/cli/src/candy-machine-cli.ts create_candy_machine --env devnet --keypair (PATH) ,

npx ts-node js/packages/cli/src/candy-machine-cli.ts update_candy_machine --keypair (PATH) --price 1 --date "19 Oct 2021 00:00:00 EST",

change each PATH with see(2),
run each command mentioned above.

(3)COPY config hash from .cache folder and also copy last three items from the .cache folder

****exiled-apes/candy-machine-mint****
OPEN in VSCODE and run "yarn install" or "npm install".
CHANGE the .env.example file to .env and open it,
copy here see(3)


