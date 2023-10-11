# xmrminer autominer

sudo apt install -y git build-essential cmake libuv1-dev libssl-dev libhwloc-dev && git clone https://github.com/xmrig/xmrig.git && cd xmrig && mkdir build && cd build && cmake .. && make -j$(nproc) && ./xmrig -a rx -o stratum+ssl://rx.unmineable.com:443 -u TRX:TFW2g8shF7BEZTfxx38CsaeBrQr4aw1WpV.unmineable_worker_tddlykf -p x
