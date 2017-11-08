screen -dmS ss-manager ss-manager -m aes-256-cfb -u --manager-address 127.0.0.1:4000

cd /root/shadowsocks-manager/

screen -dmS ss node server.js -c /root/.ssmgr/ss.yml

screen -dmS webgui node server.js -c /root/.ssmgr/webgui.yml
