# Installing / Upgrading & Downgrading PHP in UBUNTU 


# Installing PHP

- Installing necessary packages 

        sudo apt install software-properties-common ca-certificates lsb-release apt-transport-https apache2

- Add repoitory 

        sudo add-apt-repository ppa:ondrej/php

        -------------NOTE--------------

        CAVEATS:
        1. If you are using php-gearman, you need to add ppa:ondrej/pkg-gearman
        2. If you are using apache2, you are advised to add ppa:ondrej/apache2
        3. If you are using nginx, you are advised to add ppa:ondrej/nginx-mainline
           or ppa:ondrej/nginx

- Perform update 

        sudo apt update


- Lets install a Particular version 

        sudo apt install php8.0

        sudo apt install php8.0-mysql php8.0-mbstring php8.0-xml php8.0-curl php8.0-gd


- check the version 

        php -v

- Check for different versions of php


        sudo update-alternatives --config php
        # as u didnt installed any other version u cant find any other version 

        #output
        ----------------------------------------------------------------

        root@xxxx:/home/ubuntu# sudo update-alternatives --config php
        There is only one alternative in link group php (providing /usr/bin/php): /usr/bin/php8.0
        Nothing to configure.

        ----------------------------------------------------------------


### Upgrade / Downgrade PHP versions : [Click here ](./UpgradeORDowngrade.md)