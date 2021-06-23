# softether_logpurge by Syed Kashif Ejaz
wget --no-check-certificate 'https://drive.google.com/file/d/1R3sCHyc8lRMFarYOgLOTuYBaK8WdcVsb/view?usp=sharing' -O /root/softetherlogpurge.sh
dos2unix /root/softetherlogpurge.sh
chmod +x /root/softetherlogpurge.sh
#Run Crontab
crontab -e
#add the tab
* * * * * /root/softetherlogpurge.sh >/dev/null 2>&1
