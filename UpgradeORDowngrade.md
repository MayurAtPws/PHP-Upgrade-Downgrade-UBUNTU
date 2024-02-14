## Upgrade and Downgrade PHP

- First install a another version of PHP

        sudo apt install php8.2

        sudo apt install php8.2-mysql php8.2-mbstring php8.2-xml php8.2-curl php8.2-gd


- Now check the available versions to upgrade or downgrade

        sudo update-alternatives --config php

        -----------------------------------------
        #output


        There are 2 choices for the alternative php (providing /usr/bin/php).

        Selection    Path             Priority   Status
        ------------------------------------------------------------
        * 0            /usr/bin/php8.2   82        auto mode
        1            /usr/bin/php8.0   80        manual mode
        2            /usr/bin/php8.2   82        manual mode

        Press <enter> to keep the current choice[*], or type selection number: 

        -----------------------------------------

- Choose the Number of the PHP version that u wish to use and enter

- Disable the unused version & Enable the Current version u need

        #disable 8.2
        sudo a2dismod php8.2

        #enable 8.0        
        sudo a2enmod php8.0 

- If u are using apache , restart it


        systemctl restart apache2

