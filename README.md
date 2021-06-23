# softether_logpurge by Syed Kashif Ejaz
#download the file
wget --no-check-certificate 'https://drive.google.com/file/d/1R3sCHyc8lRMFarYOgLOTuYBaK8WdcVsb/view?usp=sharing' -O /root/softetherlogpurge.sh
#convert it for unixware
dos2unix /root/softetherlogpurge.sh
#make it executeable
chmod +x /root/softetherlogpurge.sh
#Run Crontab
crontab -e
#add the tab
* * * * * /root/softetherlogpurge.sh >/dev/null 2>&1
