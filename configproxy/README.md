#Config proxy for BBB

- Install shadowsocks:
```
sudo apt-get install python-pip
sudo apt-get install shadowsocks
sudo sslocal -c shadowsocks.json -d start
```

- Convert ss5 proxy to http proxy
```
sudo apt-get install polipo
sudo cp config /etc/polipo/
sudo service polipo restart
curl ifconfig.me
```
-- use http proxy to run some cmd:
```
sudo http_proxy=http://localhost:8123 apt-get update
```
