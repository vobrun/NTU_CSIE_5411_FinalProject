# Mobile and Pervasive Intelligence
## Raspberry Pi
- Ensure Raspberry Pi and Device are in same network
- Get IP address of raspberry pi

```
ssh team3_Pi1@192.168.192.1
```

Terminal 1
```
cd openvpn_client
sudo openvpn --config test.ovpn
```


Terminal 2
```
source venv/bin/activate
```

```
python3 -m streamlit run website.py --server.address 0.0.0.0 --server.port 8501
```

## Server:
```
ssh team3@team3.pailab.csie.ntu.edu.tw
```

```
cd ~/final_project/server
```

```
source venv/bin/activate
```

```
python3 server.py
```

## User device
- Enable Camera for Website

### Enabling camera on chrome ([Source](https://medium.com/@Carmichaelize/enabling-the-microphone-camera-in-chrome-for-local-unsecure-origins-9c90c3149339))
- Go to `chrome://flags/#unsafely-treat-insecure-origin-as-secure`
- enable the `Insecure origins treated as secure` section
- Add Link
- Restart Chrome
