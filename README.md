# moviePHP

## installation symfony
probleme: want to update my php7.0 to php 7.4  
solution: https://php.watch/articles/Ubuntu-PHP-7.4

probleme: the official site php command does not work for me php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"  
solution: curl https://getcomposer.org/installer > composer-setup.php  //use the curl to getfile and write the output into composer-setup.php

probleme: somfony requirement not reached, caused by the manque of php extension  
solution: sudo apt-get install php7.4-cli php7.4-fpm php7.4-bcmath php7.4-curl php7.4-gd php7.4-intl php7.4-json php7.4-mbstring php7.4-mysql php7.4-opcache php7.4-sqlite3 php7.4-xml php7.4-zip

probleme: The "https://packagist.org/packages.json" file could not be downloaded: failed to open stream: No connection could be made because the target machine actively refused it.   
solution: sudo sh -c "echo 'precedence ::ffff:0:0/96 100' >> /etc/gai.conf" //Operation timed out (IPv6 issues)
