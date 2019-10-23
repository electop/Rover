## Prerequites
```
pip --version
sudo python -m pip uninstall pip setuptools
sudo python3 -m pip uninstall pip setuptools
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
