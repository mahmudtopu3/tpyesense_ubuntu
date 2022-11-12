# typesense_ubuntu
Install typesense on Ubuntu

## curl -O https://dl.typesense.org/releases/0.23.1/typesense-server-0.23.1-amd64.deb
## sudo chown _apt typesense-server-0.23.1-amd64.deb
## sudo apt install ./typesense-server-0.23.1-amd64.deb
## nano /etc/typesense/typesense-server.ini
## Change ip and api key
``api-address = ....
api-port = 8108
peering-address=.....
data-dir = /var/lib/typesense
api-key = xyz
log-dir = /var/log/typesense
enable-cors=true``


## service typesense-server start/restart/stop 

## sudo systemctl status typesense-server.service

## in postman http://128.199.33.211:8108/collections/  try with headers x-typesense-api-key=xyz and Content-Type=application/json
