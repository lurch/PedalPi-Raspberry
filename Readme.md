# PedalPi - Raspberry

PedalPi implementation for Raspberry

## To "install" (use for development)

```bash
git clone --recursive https://github.com/PedalPi/WebService

sudo pip3 install virtualenv

virtualenv PedalPi
source ./PedalPi/bin/activate

pip3 install -r requirements.txt
```

## To run

```
source ./PedalPi/bin/activate
python3 start.py
```

## To send your changes from your PC to Raspberry

```
rsync -Cravzp --delete-after <path to project>/PedalPi-Raspberry/ pi@<IP address>:<Raspberry path> --exclude-from=.gitignore
```
