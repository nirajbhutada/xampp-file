# xampp-file
C:\xampp\apache\conf\extra\httpd-vhosts.conf
NameVirtualHost *:80
NameVirtualHost *:1005
NameVirtualHost *:8080



<VirtualHost *:80>
    DocumentRoot "C:\xampp\htdocs"
    ServerName localhost
</VirtualHost>


<VirtualHost *:8080>
    DocumentRoot "D:\project\Source\rwd-account-center\sprint3"
    ServerName localhost
    <Directory "D:\project\Source\rwd-account-center\sprint3">
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>



<VirtualHost *:1005>
    DocumentRoot "D:\project\Source\SMC\SMC - Sprint 2"
    ServerName localhost
    <Directory "D:\project\Source\SMC\SMC - Sprint 2">
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>





##<VirtualHost *:80>
    ##ServerAdmin webmaster@dummy-host2.example.com
    ##DocumentRoot "C:/xampp/htdocs/dummy-host2.example.com"
    ##ServerName dummy-host2.example.com
    ##ErrorLog "logs/dummy-host2.example.com-error.log"
    ##CustomLog "logs/dummy-host2.example.com-access.log" common
##</VirtualHost>



