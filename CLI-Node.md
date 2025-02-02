# CLI Node Run Full Guide (PC and VPS for Both)

1️⃣ Dependencies for WINDOWS & LINUX & VPS
```
sudo apt update
sudo apt upgrade -y
```

For VPS Only
```
apt install screen -y
```

2️⃣ Download Some Files
```
curl https://download.hyper.space/api/install | bash
```
```
source /root/.bashrc
```

For VPS Only
```
screen -S hyperspace
```
```
source /root/.bashrc
```

3️⃣ Put Your Old Private Key
```
nano .pem
```
Then save - CTRL+X Then Enter Y Then Enter

4️⃣ Start Node
```
aios-cli start
```

For VPS Only
```
PRESS CTRL+A+D (to run ur node continuously)
```

## Open Another Window for WSL or VPS

For VPS Only
```
screen -S cli-hyperspace
```

### Check Your Preference Model
```
aios-cli models list
```

1️⃣ Choose Your Tier (currently ranging from best to worst as 1-5)
```
aios-cli hive select-tier 5
```

2️⃣ Download Tier Model
```
aios-cli models add hf:TheBloke/phi-2-GGUF:phi-2.Q4_K_M.gguf
```

3️⃣ Registered Your Tier
```
aios-cli hive connect
```
```
aios-cli hive select-tier 5
```

4️⃣ To Check Your Current Multiplier and Points
```
aios-cli hive points
```

5️⃣ Check Your Node Status
```
aios-cli status
```

## If Node Not Working Then Kill Node and Reconnect
```
aios-cli kill
```
Then Start Node

## Import Your Private and Public Key
```
aios-cli hive whoami
```


