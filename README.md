# mnscripts
Masternode scripts for Arionum

So, this is a pretty junky thing I threw together so I can have all of my masternodes get their earnings sent to a centralized wallet.  I did this because I used the web wallet and yeah, you guys know what happened there.  This does NOT need to be ran on the masternodes.  I instead have all of my wallets being hosted on more secure local server that doesn't do a lot else besides have cli wallets.

Guide:
You will need to have the CLI wallet up and running (correct php...etc)
You will need to have your wallet unencrypted for my script to work, I may change that later.
The wallet.aro file and the CLI wallet both need to be in the same folder
Copy the file called script from this repository to your wallet folder
type chmod +x script
edit the script so that your wallet is where it says you need it
type ./script
success!  

Bonus:  if you want to automate this, use cron. 
1.  type crontab -e
2.  add the following to the end of the file
0 * * * * /absolute/path/to/your/script
for instance, mine looks like 0 * * * * /home/icusu/wallets/wallet1/script

This will have the script run hourly.  Yay
