# TorNet
TorNet is a cybersecurity and privacy project that explores anonymous networking through Tor, showcasing how onion routing enhances user anonymity and protects against network surveillance.
Steghide Tutorial

Basic Steps:
```bash
sudo apt update
```
```bash
sudo apt upgrade -y
```
(This Ensures system has latest security patches and Software version)

Install Tor:
```bash
sudo apt install tor
```
After Installation:
1) Install Python3:
```bash
sudo apt install python3
```
2) Create a virtual environment for TorNet: This would create a seperate python environment for TorNet, Isolated from the system's Global python
```bash
python3 -m venv tornet-venv
```
3) Activate tornet-venv:
```bash
source tornet-venv/bin/activate
```
4) Install TorNet inside the venv:
```bash
pip install tornet
```
5) Go to your Browser Settings -----> Network Settings: Change to manual proxy configuration and type in the following:

SOCKS Host
```bash
127.0.0.1
```
Port
```bash
9050
```
6) Run TorNet with Time control:
```bash
tornet --interval 12 --count 0
```
7) TorNet Runs
