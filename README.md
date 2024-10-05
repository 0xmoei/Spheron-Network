# Spheron Network Worker Node
Spheron’s Fizz Nodes offer a low-barrier entry point for anyone looking to contribute resources to Spheron’s decentralized compute network—and earn ongoing rewards for their contributions.

Whether you're looking to run a basic CPU configuration or a powerful GPU setup, this guide will walk you through the entire process


# Step-by-Step Guide to Run Fizz Node

## Hardware Requirement
![image](https://github.com/user-attachments/assets/d9d9f0a7-a2f2-41da-8194-16d6dd4b8a00)

## Register Fizz Node
1. Open Your Browser: Navigate to https://fizz.spheron.network
2. Sign up or log in through Gmail or Github
3. Click on the “Register New Fizz Node” Button and Connect your wallet

![image](https://github.com/user-attachments/assets/2876dc7d-dc59-460c-9a0d-f42ce0ea4343)

4. Select your node's OS, resources, Region, Payment Tokens, and Provider ( I selected highest tier provider )

![image](https://github.com/user-attachments/assets/536c09d7-1af6-4832-9b4c-33b9861fecd6)
![image](https://github.com/user-attachments/assets/2ce43536-0cbd-435a-baf3-9beb0c05c645)

5. Click **“Register Your Fizz Node“**, To complete the registration, you'll need some ETH on the Spheron chain for gas fees. If you don't have any, you can get some from our faucet at https://faucet.spheron.network

![image](https://github.com/user-attachments/assets/afcd4cd4-240d-46aa-a5d8-6d35bdea0741)


## Run the Fizz Node
1. In setup page for your registered nod, You should find a link to download the `fizzup.sh` script

![image](https://github.com/user-attachments/assets/3052022b-2a14-42a7-8613-bf6ea5624a08)

2. Download the `fizzup.sh` script to your PC. Send it to your VPS using `Mobaxterm` or `Termius` Clients

3. Install Docker
```console
sudo apt update -y && sudo apt upgrade -y
for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do sudo apt-get remove $pkg; done

sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg

echo \
  "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt update -y && sudo apt upgrade -y

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

sudo chmod +x /usr/local/bin/docker-compose

# Docker version check
docker --version
```

4. Give persmissions to script
```console
# assuming I transfered the script to the main (root) folder of server
chmod +x /root/fizzup.sh
```

5. Run Fizz Node Script
```
sh /root/fizzup.sh
```






