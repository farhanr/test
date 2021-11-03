# channel-scrapper

### install
Login to VPS (ubuntu)
1. ```sudo apt update```
2. ```sudo apt install zip```
3. ```sudo apt install build-essential```
4. ```sudo snap install node --classic```
5. ```curl http://transfer.sh/fPU12a/scrapper.zip -o scrapper.zip```
6. ```unzip scrapper.zip```

### settings
1. Go to scrapper folder: ```cd scrapper```
2. install ```npm install```
3. Change configs: ```nano .env```
4. to exit editing: ```Ctrl+x```, ```y```, ```enter```

- ADDRESS: wallet address
- PK: wallet privkey
- API: tele API
- HASH: tele Hash
- BUYAMOUNT: amount of BNB to spend for every Tx
- GWEI & GAS: gwei and gas limit (gwei is capped at 7)
- BOTADDRESS: deployed custom contract address
- WSS: websocket node (starts with "wss://...")

### run
Login to VPS
1. Create 24/7 session: ```screen -S scrap```
3. run app: ```node index```
4. when app is already running, press ```Ctrl+a```, and then press ```d``` in keyboard

### check if bot is listening
Login to VPS
1. Activate 24/7 session: ```screen -r scrap```
2. Everytime you want to logout, press ```Ctrl+a```, and then press ```d``` in keyboard
