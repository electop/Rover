## Prerequites
```
pip --version
sudo python3 -m pip uninstall pip setuptools
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
sudo python get-pip.py
sudo apt install python3-pip
pip3 --version
pip --version
python -m ensurepip --default-pip
pip install virtualenv
git clone https://github.com/Roger-random/SGVHAK_Rover.git
cd SGVHAK_Rover
git branch -a
git checkout development
cp config_sawppy.json ../SGVHAK_Rover/
cp init.sh ../SGVHAK_Rover/
cp config_sawppy.json config_roverchassis.json 
python -m virtualenv venv
. venv/bin/activate
sudo pip install -e .
sudo ./start.sh 
```
https://hackaday.io/project/158208-sawppy-the-rover<br>
https://github.com/Roger-random/SGVHAK_Rover<br>
https://github.com/Roger-random/Sawppy_Rover/blob/master/docs/SGVHAK%20Rover%20Software.md

### start.sh
```
export FLASK_APP=SGVHAK_Rover
#export FLASK_DEBUG=1
#flask run
flask run --host=0.0.0.0 &
```

### init.sh (e.g.) init.sh 300
```
#!/bin/bash
echo "arg: $1"
sudo python3 SGVHAK_Rover/lewansoul_wrapper.py --id 23 --move $1
sudo python3 SGVHAK_Rover/lewansoul_wrapper.py --id 29 --move $1
sudo python3 SGVHAK_Rover/lewansoul_wrapper.py --id 24 --move $1
sudo python3 SGVHAK_Rover/lewansoul_wrapper.py --id 26 --move $1
```
