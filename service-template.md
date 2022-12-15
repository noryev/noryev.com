[Unit]
Description=ipfs daemon

[Service]

ExecStart=/usr/local/bin/ipfs daemon --enable-gc

Restart=always

User=ubuntu

Group=ubuntu

Environment="IPFS_PATH=/home/ubuntu/data/ipfs"

[Install]

WantedBy=multi-user.target
s