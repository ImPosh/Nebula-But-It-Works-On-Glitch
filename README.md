<div align=center> <img src='https://nebulaproxy.nebula.bio/images/logo.png' width="100px" height="100px">
Nebula
Nebula Web is an official flagship of Nebula Services. Nebula Web is a stunning and sleak webproxy with support for hundreds of popular sites, and partial support for WebRTC, used in GfN. With Nebula Web, the sky is the limit. Enjoy. </div>
Features
Stunning UI with multiple themes
XOR/b64 Encrypts all traffic sent from Nebula
Hides your IP from sites
List of officially supported sites
limited mobile support
StealthMode (buffed about:blank cloaking)
Self Hosting
$ git clone https://github.com/NebulaServices/Nebula.git
$ cd Nebula
$ npm ci
$ npm start
Tech Stack
HTML, JS, CSS
Partical.JS
UV Backend Proxy
Osana Backend Proxy
Server: Bare server on Node
Support
For support, email chloe@nebula.bio or join our discord: discord.nebula.bio

Demo
Click here to see a demo of Nebula

Deployment
Quick Deployment Options
Deploy to Heroku
Run on Replit
Remix on Glitch
Deploy to IBM Cloud
Deploy to Amplify Console
Run on Google Cloud
Deploy on Railway
Deploy To Koyeb

Advanced Deployment
Initial configuration
credits to @ProgrammerIn-wonderland for writing this wonderful tutorial (which can also be found in the docs :)

Create an account at https://www.cloudflare.com/
Create an account at https://www.freenom.com/ (or any registrars)
Find a free domain name at Freenom
Click checkout
Select (12 Months @ FREE)
Select "Use DNS"
Select Use your own DNS
Go to cloudflare, click add new site, and enter the free domain name
Select "Free Plan"
Click continue, ignore DNS
Copy the name servers cloudflare gives you
Go back to your Freenom tab, enter in the name servers which cloudflare gave you
You can keep IP blank
Click continue
Click complete order
Go back to cloudflare tab, click "Check Nameservers"
Select DNS on your right bar
Enter in the IP of the server which will be hosting Nebula
Target will be @
Click Enable proxy (little gray cloud icon, if active its orange)
Select SSL/TLS in your right bar
Click "Flexible"
Server configuration
SSH into the server you'll be using, I'll assume its running Ubuntu 22.04 (though the commands are the same for debian 10+ versions, and Ubuntu versions 20.04+)
run
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - \ &&
sudo apt-get install -y nodejs npm
git clone https://github.com/NebulaServices/Nebula.git
cd Nebula
npm i
npm ci
sudo nohup PORT=80 node . &
Make sure your firewall is configured to let through port 80 traffic!
Note: Server will need to run cd Nebula && sudo nohup PORT=80 node . & on reboot (Nebula's license is now GNU AGPL V3 as of v7.10)

Acknowledgements
UV (one of the back-end proxy we use)
Osana (one of the back-end proxy we use)
Bare Server
Partical.JS (v4, 5, 6.1 &< only)
License
Copyright Nebula Services 2021 - Present
This project uses the AGLP GNU V3 license.
