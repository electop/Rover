## Prerequites
```
pip --version
sudo python3 -m pip uninstall pip setuptools
wget https://bootstrap.pypa.io/get-pip.py -o get-pip.py
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
