# Hello
Install homebridge on PI3

## install latest node

sudo apt-get remove nodejs nodejs-legacy nodered
curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -
sudo apt-get install -y nodejs

sudo npm install npm@latest -g


sudo npm install -g node-gyp
sudo npm install -g npm-check
sudo npm install -g npm-check-updates

node -v
`v9.11.1`

## install homebridge

sudo npm install -g --unsafe-perm homebridge

## reset homebridge

rm -rf .homebridge/persist/


##  check the status of the service by calling
Status : `systemctl status homebridge`

Detail : `journalctl -u homebridge.service`

Service : 

`sudo systemctl stop homebridge`

`sudo systemctl start homebridge`
