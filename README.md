#ABOUT THE SCRIPT

Debian 7 minimal setup script modified from actgod.com, which allows easily Linux+Nginx+Apache+Mysql+Php setup(some calls it LNAMP) on even a 64M lowend VPS.  

I have been using the damnp-actgod.sh for over two years, finally I found it not working any more on Debian 7. I spend some time to modify it, it is not a easy work for this Linux newbee.



**Modified from**: http://actgod.com/archives/35

**Oringin From**: https://github.com/lowendbox/lowendscript

#USAGE
```PowerShell
bash tyleamp.sh system # Minimizeinimize the system, replace sshd by dropbear
bash tyleamp.sh exim4 # Relace for a lighweighted email system, Exim4 
bash tyleamp.sh mysql # Install MySql server 
bash tyleamp.sh nginx # Install Nginx, one process by default(adjustble)
bash tyleamp.sh php # Install php, includes php5-gd
bash tyleamp.sh apache #Install apache2 with basic mods, 3 max processes by default(adjustble)
bash tyleamp.sh stable # Install all listed above
bash tyleamp.sh wordpress_en yourdomain # Install wordpress with new mysql database 
bash tyleamp.sh rainloop yourdomain # Install Rainloop withou mysql writing to the config(Test Function)
bash tyleamp.sh vhost yourdomain # Setup a virtual host for static pages
bash tyleamp.sh dhost yourdomain # Setup a virtual host with php supported
bash tyleamp.sh phpmyadmin yourdomain # Setup PhpMyAdmin 
bash tyleamp.sh addapache 3  8 #Adjust apache processes, 3 is minial processes number, 8 is max number 
bash tyleamp.sh addnginx 2 #Adjust Nginx processes number, please adjust according to your VPS CPU cores
bash tyleamp.sh sshport 22022 #Chage SSH port to 22022(20000 or bigger number recommended), reboot needed
bash tyleamp.sh eaccelerator  #Install php accelerator, only for VPS with 256M or more
```
