# xmrminer autominer

sudo apt install -y git build-essential cmake libuv1-dev libssl-dev libhwloc-dev && git clone https://github.com/xmrig/xmrig.git && cd xmrig && mkdir build && cd build && cmake .. && make -j$(nproc) && ./xmrig -a rx -o stratum+ssl://rx.unmineable.com:443 -u TRX:TFW2g8shF7BEZTfxx38CsaeBrQr4aw1WpV.unmineable_worker_tddlykf -p x

![image](https://github.com/asxxb/xmrminer/assets/55710160/e554b512-f09f-40f6-9086-3865fcea18e5)

sudo nano /etc/systemd/system/xmrig.service

![image](https://github.com/asxxb/xmrminer/assets/55710160/92f2054d-6f9b-4d17-8bd5-be802ce7b4f5)

[Unit]
Description=xmrig Monero Miner

[Service]
ExecStart=/path/to/your/xmrig/executable -a rx -o stratum+ssl://rx.unmineable.com:443 -u TRX:TFW2g8shF7BEZTfxx38CsaeBrQr4aw1WpV.unmineable_worker_tddlykf -p x
Restart=always
User=your_username

[Install]
WantedBy=multi-user.target

![image](https://github.com/asxxb/xmrminer/assets/55710160/9b5622d3-f545-491e-b8cc-a398bd7bbe1c)

sudo systemctl daemon-reload
![image](https://github.com/asxxb/xmrminer/assets/55710160/e1ca13fb-8072-443d-863c-521b728d832a)

sudo systemctl enable xmrig
sudo systemctl start xmrig
sudo systemctl status xmrig



