# main
screen -s myscreen

Нажать ctrl+c потом CTRL+A+d

cd pathfinder

git fetch

git checkout v0.1.8-alpha

git clone --branch v0.1.8-alpha https://github.com/eqlabs/pathfinder.git

screen -s myscreen

cd $HOME/pathfinder/py

python3 -m venv .venv

source .venv/bin/activate

PIP_REQUIRE_VIRTUALENV=true pip install -r requirements-dev.txt

cargo build --release --bin pathfinder

