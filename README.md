# Nodepay Automate with Proxies 
Automate farming Nodepay Network using proxies. Important! Please read the Information below:
- Old version is not working anymore, Please use ``runv2.py`` instead!
- Now this script support Windows without [WSL](https://learn.microsoft.com/en-us/windows/wsl/install)
- This script support multiple accounts. Support socks and http proxies. Using 3 proxies for each accounts.
<!--For Windows users please use [WSL](https://learn.microsoft.com/en-us/windows/wsl/install)-->
<!--- Latest curl_cffi modules (for impersonate chrome131 version) ``curl_cffi==0.8.0b7`` isn't updated from Windows Python Library server. I already tried impersonate chrome110 version and others but still getting error, stable impersonate is chrome131 version.
~Please use the bypass version. I found Nodepay's real IP host to make farming easier without being blocked by Cloudflare protection.~
- This bot only support for Linux and [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) Windows for now, for Termux use [tutorial](https://github.com/im-hanzou/nodepay-automate?tab=readme-ov-file#termux) below.-->
## Tools and components required
1. Nodepay Account | Register: [https://app.nodepay.ai/register](https://app.nodepay.ai/register?ref=ZUCBuJaIoBXLE6J)
2. VPS (OPTIONAL) and Python3
3. Proxies
## Buy Proxies
- Free Proxies Static Residental: 
1. [WebShare](https://www.webshare.io/?referral_code=p7k7whpdu2jg)
2. [ProxyScrape](https://proxyscrape.com/?ref=odk1mmj)
3. [MonoSans](https://github.com/monosans/proxy-list)
- Paid Premium Static Residental:
1. [922proxy](https://www.922proxy.com/register?inviter_code=d03d4fed)
2. [Proxy-Cheap](https://app.proxy-cheap.com/r/JysUiH)
3. [Infatica](https://dashboard.infatica.io/aff.php?aff=544)
# Setup Tutorial
- Open [Nodepay](https://app.nodepay.ai/register?ref=ZUCBuJaIoBXLE6J) and login to dashboard
- Press F12 or CTRL + SHIFT + I
- Select CONSOLE and type ```allow pasting``` and press enter
<!-- - Important! Make sure you installed Nodepay Extension in your Browser and must be Connected after getting token!, Download Extension: [Nodepay Extension](https://chromewebstore.google.com/detail/nodepay-extension/lgmpfmgeabnnlemejacfljbmonaomfmm) -->
![0001](https://github.com/im-hanzou/getgrass_bot/blob/main/pasting.JPG)
- Then type ``localStorage.getItem('np_token')`` and press enter
![0002](https://github.com/im-hanzou/getgrass_bot/blob/main/nodepaytoken.png)
- The text that appears is your nodepay token and copy the text
# Components installation
### LINUX

```bash
git clone https://github.com/ZoroJooo/nodepay
cd nodepay
```
- Installing requirements:
```bash
apt install python3.12-venv
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install -r requirements.txt
```
# Run the Script
- Replace the proxies example in ```proxies.txt``` to your own proxies, please use only 3 proxies with proxies. If you run multiple accounts make sure you have 3 proxies for each accounts.
- For multi accounts, insert your tokens perlines in file ``tokens.txt``
<!-- ## Run command Windows
- Run for original server - version 2:
```bash
python runv2.py
```
>Press Enter, Select 1 then insert your nodepay token
- Run for original server - version 2 - multi accounts:
>Make sure you have tokens in ``tokens.txt`` before
```bash
python runv2.py
```
>Press Enter then Select 2 -->
## Run command

### Linux Distros
- Run for original server - version 2:
```bash
python3 runv2.py
```
>Press Enter, Select 1 then insert your nodepay token
- Run for original server - version 2 - multi accounts:
>Make sure you have tokens in ``tokens.txt`` before
```bash
python3 runv2.py
```
>Press Enter then Select 2
<!-- - ~Run for original server~:
```bash
python run.py
```
>~Press Enter then insert your nodepay token~ Not working anymore, please use ``runv2.py``
- ~Run for bypass server~:
>~Use this script if you getting errors like ```Error during API call: 403 Client Error: Forbidden for url```~. Not working anymore, please use ``runv2.py``
```bash
python run-bypass.py
```
>~Press Enter then insert your nodepay token~ Not working anymore, please use ``runv2.py``
- ~Run for multi bypassed server~:
```bash
python run-multi-bypass.py
```
>Not working anymore, please use ``runv2.py`` -->
# Operating status
If the following log appears, it means it is running successfully.
```bash
[2024-12-02 14:54:54] [INFO] Account: user@email.com | Browser ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP Score: 99
[2024-12-02 14:54:58] [INFO] Account: user@email.com | Browser ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP Score: 86
[2024-12-02 14:54:59] [INFO] Account: user@email.com | Browser ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP Score: 92
[2024-12-02 14:55:02] [INFO] Account: user@email.com | Browser ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP Score: 81
[2024-12-02 14:55:11] [INFO] Account: user@email.com | Browser ID: xxxxxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxx | IP: 127.0.0.1 | IP Score: 82
```
# Notes
- Run this script, and it will update your referral code to my invite code if you don't have one.
- One account only can connect with 3 Proxies. If you run multiple accounts make sure you have 3 proxies for each accounts.
- If you run the script and still got error, please use paid proxies cause every free proxies not all supported.
- You can just run this script at your own risk, I'm not responsible for any loss or damage caused by this script. This script is for educational purposes only.
<!-- - Feel free to enjoy and recode or create new bots using the Nodepay API with direct IP that I found. -->

