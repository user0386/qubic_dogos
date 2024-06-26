## Upgrade OS
```
upgrade && sreboot
```
> minimal DogOS version 2.49
<br />

# Qubic for GPU dogos profiles
```
{"name":"Qubic GPU","coin":"custom","wallet":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6IjkyZDJkYTAyLTk1ODYtNDg1Ny05MDRjLWIxNGRkNzkyMjE2MiIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMDkzODE0OCwiZXhwIjoxNzQyNDc0MTQ4LCJpYXQiOjE3MTA5MzgxNDgsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.ADhZUmOepASLjADD4Zwt-SaNHUVPFLjksb1zxWeXkJ2BRYqNdb_6-Wsr_M-nsxGoABJbMc2ROYVDXks7LWyO9Q","pool":"https://mine.qubic.li","miner":"custom","addition":"url_qli https://dl.qubic.li/downloads/qli-Client-1.9.5-Linux-x64.tar.gz\n{\n  \"Settings\": {\n    \"baseUrl\": \"https://mine.qubic.li\",\n    \"trainer\": {\n      \"cpu\": false,\n      \"gpu\": true,\n      \"gpuVersion\": \"CUDA12\"\n    },\n    \"checkUpdateEnabled\": true,\n    \"autoupdateEnabled\": false\n  }\n}","fork":"latest","custom_url":"https://github.com/user0386/qubic_dogos/raw/main/qubic_dogos_gpu.tar.gz"}
```

# Qubic for CPU dogos profiles
```
{"name":"Qubic CPU","coin":"custom","wallet":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6IjkyZDJkYTAyLTk1ODYtNDg1Ny05MDRjLWIxNGRkNzkyMjE2MiIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMDkzODE0OCwiZXhwIjoxNzQyNDc0MTQ4LCJpYXQiOjE3MTA5MzgxNDgsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.ADhZUmOepASLjADD4Zwt-SaNHUVPFLjksb1zxWeXkJ2BRYqNdb_6-Wsr_M-nsxGoABJbMc2ROYVDXks7LWyO9Q","pool":"https://mine.qubic.li","miner":"custom","addition":"url_qli https://dl.qubic.li/downloads/qli-Client-1.9.5-Linux-x64.tar.gz\namountOfThreads -1\nhugePagesByNproc true\nhugePages_ratio 104\n{\n  \"Settings\": {\n    \"baseUrl\": \"https://mine.qubic.li\",\n    \"trainer\": {\n      \"cpu\": true,\n      \"gpu\": false,\n      \"cpuVersion\": \"AVX2\" \n    },\n    \"allowHwInfoCollect\": true,\n    \"checkUpdateEnabled\": true,\n    \"autoupdateEnabled\": false\n  }\n}","fork":"latest","custom_url":"https://github.com/user0386/qubic_dogos/raw/main/qubic_dogos_cpu.tar.gz"}
```

### Available options
| Parameter | Value |
|----------------|:---------:|
| overwrite_appsettings_json | true/false |
| url_qli | url qubic-li client |
| alias | name/no parameter |
| autoupdateEnabled | true/false |
| checkUpdateEnabled | true/false |
| allowHwInfoCollect | true/false |
| amountOfThreads | negative numbers/positive numbers/no parameter for all cores |
| hugePagesByNproc | true |
| hugePages | numbers |
| hugePages_ratio | numbers |

<br />
<br />
<br />
<br />

#### Update file cpu/miner
```
wget -O /dog/miners/custom/qubic_dogos_cpu/miner https://raw.githubusercontent.com/user0386/qubic_dogos/main/cpu/miner
```
#### Update file cpu/stats
```
wget -O /dog/miners/custom/qubic_dogos_cpu/stats https://raw.githubusercontent.com/user0386/qubic_dogos/main/cpu/stats
```

#### Update file gpu/miner
```
wget -O /dog/miners/custom/qubic_dogos_gpu/miner https://raw.githubusercontent.com/user0386/qubic_dogos/main/gpu/miner
```
#### Update file gpu/stats
```
wget -O /dog/miners/custom/qubic_dogos_gpu/stats https://raw.githubusercontent.com/user0386/qubic_dogos/main/gpu/stats
```

#### Full re install
```
getminer custom -f && miner restart
```
<br />
to select the desired version and config, visit https://github.com/qubic-li/client
<br />
<br />

-----------

## Qubic-Solutions rqiner
```
{"name":"Qubic Rqiner CPU","coin":"custom","wallet":"QUBIC_WALLET","miner":"custom","addition":"url_miner https://github.com/Qubic-Solutions/rqiner-builds/releases/download/v0.3.17/rqiner-x86\nthreads -1","fork":"latest","custom_url":"https://github.com/user0386/qubic_dogos/raw/main/rqiner_dogos.tar.gz"}
```
to select the desired version, visit  https://github.com/Qubic-Solutions/rqiner-builds/releases 

<br />
<br />
