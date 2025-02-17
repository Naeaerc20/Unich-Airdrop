# Unich-Airdrop

Unich-Airdrop is a Node.js automation script that interacts with the Unich API to perform daily mining activation and auto-complete social tasks for multiple accounts. The script uses user-provided proxies to route each account’s requests, ensuring that each account uses its designated proxy.

---

## Features

- **Daily Mining Activation:**  
  Automatically sends mining activation requests for each account using its designated proxy. After all accounts are processed, the script “rests” for 24 hours before reactivating the mining nodes automatically.

- **Auto Complete Tasks:**  
  Retrieves available social tasks for each account. Unclaimed tasks are completed automatically using the account’s username as evidence. Once processed, you can press **ENTER** to return to the main menu. Each account’s requests are routed through its assigned proxy.

- **Proxy Assignment:**  
  Proxies are defined in a `proxies.txt` file. Each account (from `users.json`) is assigned a proxy based on its order (ID 1 uses the first proxy, ID 2 uses the second, etc.).

---

## Requirements

- Node.js (v12 or later; tested on v20.15.1)
- NPM

### Dependencies

- [axios](https://www.npmjs.com/package/axios)
- [colors](https://www.npmjs.com/package/colors)
- [figlet](https://www.npmjs.com/package/figlet)
- [inquirer](https://www.npmjs.com/package/inquirer)
- [console-clear](https://www.npmjs.com/package/console-clear)
- [socks-proxy-agent](https://www.npmjs.com/package/socks-proxy-agent)

---

## Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/Unich-Airdrop.git
   cd Unich-Airdrop

2. **Install packages**

   ```bash
   npm install

3. **Set accounts & proxies**

   ```bash
   nano proxies.txt
   nano users.json


Note: Set proxies from 2CAPTCHA with format "socks5://login:pass@ip:port"
Not in Unich yet? - Get started today with my link and this code - https://unich.com/en/airdrop/sign-up?ref=5AI4S4
