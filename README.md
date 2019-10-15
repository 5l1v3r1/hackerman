# Hackerman .. 

## python hacking module

![OS](https://img.shields.io/badge/Support%20-Linux%20|%20Termux-yellowgreen.svg?style=flat-square) [![Python2.7](https://img.shields.io/badge/Python-2.7-green.svg?style=flat-square)](https://www.python.org/downloads/release/python-2714/)


# The Modules :

| Name              | Description                   |
| :-------------    | :-------------                |
| `porscanner`      | Make Portscanner script       |
| `whoup`           | Show whoup in Network         |
| `xss`             | Xss Reflacted Scanner         |
| `sqli`            | SQL INJECTION Scanner          |
| `ssti`            | SSTI Scanner                  |
| `headers`         | Get HTTP Headers              |
| `make_payload`    | Make Rat Payload              |
| `make_connection` | Make Connection With Rat Victim   |
| `restart`         | restart your script           |
| `slow_print`      | print the words in slow mode     |
| `dos_attack`      | Make Dos Attack Script        |
| `scapy_dos_attack`| Make Dos Attack Script with scapy         |


# > Rat Features <img src="https://img.icons8.com/cotton/64/000000/hacking.png" width="40" height="35">

- ### Upload And Download Files
- ### Execute os Command
- ### Get Victim Address
- ### openfile in victim device
- ### open url in Victim Browser
- ### print message in Victim terminal
- ### see who is up on the victim network
- ### Take screenshot from victim device


# Examples :
- xss Scanner Script 
```python
from hackerman import xss
import sys
def logo():
        print ('''
__  __       _____          ___
\ \/ /___ __|_   _|__   ___ | |
 \  // __/ __|| |/ _ \ / _ \| |
 /  \\__ \__ \| | (_) | (_) | |
/_/\_\___/___/|_|\___/ \___/|_|

[ Coded By : hacker ]
[ version  : 0.1    ]
''')

def getarg():
        global target
        target=sys.argv[1]

logo()
getarg()
xss(target)
```
  - ## Run it 
     ```python2 main.py 'http://leettime.net/xsslab1/chalg1.php?name=5*&submit=Search' ```
  - ## The Result 
     <img src="https://i.ibb.co/SnrP8SL/Screenshot-from-2019-10-15-00-58-45.png" alt="XSS Tool">
     
     ### Note : Add * in param
     For More scan 
     ```python
     from hackerman import sqli , ssti
     sqli(target) , ssti(target)```

- Port Scanner Script
```python
from hackerman import portscanner
import sys
def logo():
        print ('''

 _ __  ___  ___ __ _ _ __  
| '_ \/ __|/ __/ _` | '_ \ 
| |_) \__ \ (_| (_| | | | |
| .__/|___/\___\__,_|_| |_|
|_|

[ Coded By : Hacker ]
[ Version  : 0.1    ]

''')

def getarg():
        global ip,port1,port2
        ip=sys.argv[1]
        port1=sys.argv[2]
        port2=sys.argv[3]

logo()
getarg()
portscanner(ip,port1,port2)
```

- ## Run it 
     ````python2 pscan.py 127.0.0.1 80 3306 ````
     
- ## The Result 
  <img src="https://i.ibb.co/dDjJrYY/Screenshot-from-2019-10-15-01-12-46.png" alt="Port Scanner Tool" >
  
  
  
# More Examples :
- ## <a href='https://github/knassar702/hackerman-tools' target='_blank'> Hackerman-Scripts</a>
      
# Installation :

## [Linux](https://wikipedia.org/wiki/Linux) [![alt tag](http://icons.iconarchive.com/icons/dakirby309/simply-styled/32/OS-Linux-icon.png)](https://fr.wikipedia.org/wiki/Linux)

- ### open your terminal
- ### enter this command
```bash
$ apt install git python2 python2-pip && git clone https://github.com/knassar702/hackerman && cd hackerman && pip2 install -r requirements.txt && python2 setup.py install && echo "from hackerman import slow_print;slow_print('Welcome in Hackerman module .. Good luck :) ..',1)" > first.py && python2 first.py
```

## Andoird <img src="https://img.icons8.com/clouds/100/000000/android-os.png">

- ### Download Termux App
- ### Enter this command
```bash
$ pkg update && pkg install python2 && pkg install git && pip2 install -r requirements.txt && python2 setup.py install && echo "from hackerman import slow_print;slow_print('Welcome in Hackerman module .. Good luck :) ..',1)" > first.py && python2 first.py
```

# License

GPL-2.0 Licence
