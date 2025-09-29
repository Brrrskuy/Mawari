# <h2 align=center> Mawari Nodes </h2>

- Buy VPS : [Skuy Vibes](https://t.me/skuyvibes/156) `<---`
- Trakteer buy Coffee : https://trakteer.id/brrrskuy/tip `<---`
-------------------------------------
### 1.Connect Wallet
`-->` [Mawari Network Testnet](https://testnet.mawari.net/) 
### 2.Claim Faucet
`-->` [Claim Faucet Mawari Testnet](https://hub.testnet.mawari.net/)
### 3.Mint Guardian NFT
`-->` [Mint 3 Guardian NFT Max](https://testnet.mawari.net/mint)

# <h2 align=center> -VPS Setup- </h2> 

### 1. Install Docker
```
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin -y
```
### 2. Enable Docker
```
sudo systemctl start docker
sudo systemctl enable docker
```
### 3. Create Directory
```
mkdir -p ~/mawari
cd ~/mawari
```
### 4. Create Screen
```
screen -S mawari
```
### 5. Setup Environment
```
export MNTESTNET_IMAGE=us-east4-docker.pkg.dev/mawarinetwork-dev/mwr-net-d-car-uses4-public-docker-registry-e62e/mawari-node:latest
```
### 6. Set your owner Address
```
export OWNER_ADDRESS=0xYourAddress
```
### 7. Running Guardian Nodes
```
docker run --pull always -v ~/mawari:/app/cache  -e OWNERS_ALLOWLIST=$OWNER_ADDRESS $MNTESTNET_IMAGE
```
### 8. Find your Burner Address
```
nano $HOME/mawari/flohive-cache.json
```
### 9. After Done Running
go to  [Mawari Licenses](https://app.testnet.mawari.net/licenses) and Delegate all 3 NFT Guardian
### 10. Send 1 Faucet to Burner Address
go to `Find your Burner Address to see Burner Address`

-------------------------------------
### Screen Command

Detached Screen press `CTRL+A+D`

See Screen `screen -r mawari`

----------------------------------------------------------
### Join Telegram Channel🚀
For Updates, Questions and other Guides Join the Community :

[Skuy Vibes](https://t.me/skuyvibes) or [Airdrop Family IDN](https://t.me/AirdropFamilyIDN)
