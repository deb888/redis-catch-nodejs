# redis-catch-nodejs
how to use redis in node js for catch purpose


for mac install 

brew install redis

lunch on pc start

ln -sfv /usr/local/opt/redis/*.plist ~/Library/LaunchAgents

using launchctl
launchctl load ~/Library/LaunchAgents/homebrew.mxcl.redis.plist


or

redis-server /usr/local/etc/redis.conf



for uninstall
$ brew uninstall redis
$ rm ~/Library/LaunchAgents/homebrew.mxcl.redis.plist

for stop 
redis-cli shutdown



For windows using linux destro


for ubuntu 

sudo apt-get install redis-server

sudo systemctl enable redis-server.service

sudo vim /etc/redis/redis.conf

//setting required for perticular redis
maxmemory 256mb
maxmemory-policy allkeys-lru

sudo systemctl restart redis-server.service
