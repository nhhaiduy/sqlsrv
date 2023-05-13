# sqlsrv
Setup SQLSRV 


sudo su
curl https://packages.microsoft.com/keys/microsoft.asc | apt-key add -
curl https://packages.microsoft.com/config/debian/11/prod.list > /etc/apt/sources.list.d/mssql-release.list
sudo apt-get update
sudo ACCEPT_EULA=Y apt-get install -y msodbcsql18

//tinh sau
sudo ACCEPT_EULA=Y apt-get install -y mssql-tools18
echo 'export PATH="$PATH:/opt/mssql-tools18/bin"' >> ~/.bashrc
source ~/.bashrc

sudo apt-get install -y unixodbc-dev
sudo apt-get install -y libgssapi-krb5-2

php81 extention

/opt/php81/lib/php/extensions/no-debug-non-zts-20210902
config ini /opt/php81/conf.d