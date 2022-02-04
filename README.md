# frida_injection
![image](https://user-images.githubusercontent.com/85984486/151764266-35ff181a-9a5f-467e-99eb-98fc5737d1d3.png)

<p align="center">
<a href="https://github.com/AbhiTheModder"><img title="GitHub" src="https://img.shields.io/badge/Abhi-TheModder-brightgreen?style=for-the-badge&logo=github"></a>
<a href="https://www.youtube.com/channel/UCtBILuQgvXHPfvOUdcmMS2Q"><img title="YouTube" src="https://img.shields.io/badge/YouTube-Abhi The MØÐÐĒR-red?style=for-the-badge&logo=Youtube"></a>
</p>

<p align="center">
<a href="https://t.me/joinchat/xP-wW-A5mIBmMjY1"><img title="Telegram" src="https://img.shields.io/badge/Telegram-black?style=for-the-badge&logo=Telegram"></a>
<a href="https://t.me/Mods_byAbhi_demandbot"><img title="Telegram Bot" src="https://img.shields.io/badge/Telegram-bot-black?style=for-the-badge&logo=Telegram_bot"></a>

## What is Frida?
Frida is a dynamic instrumentation toolkit for developers, reverse-engineers, and security researchers.

Frida allows:

1)Injection of your own scripts into black box processes.
2)Hook any function.
3)Spy on crypto APIs or trace private application code.
4)Disable SSL Pinning and root checkers. and many more things....

Frida is one of the best tools to use during an application penetration testing.
 
 ## What is this script?
 
  The script does the following:

1 Unzips the APK passed as input.
2 Asks for the architecture of the Android device. There are two options: The architecture is known, then the gadget is injected only for that architecture. The architecture is unknow, then the gadget is injected in all architectures.
3 Asks for the library to be injected, then downloads the last gadget from Frida repository and injects it.
4 Removes the old signature.
5 Generates the APK with the name my_app.apk
 
 # IDEA 
 
 Executable formats include libraries that are linked with executable. In the loading phase of the executable, the loader iterates over these libraries and map them in the memory space of the process. Once mapped it calls its constructor. The idea is to add frida-agent.so as a dependency of native libraries embedded in the APK.

### NOTE
 This tool is inspired by "https://gitlab.com/jlajara/frida-gadget-lief-injector" Jorge/Frida gadget Lief injection but with new UI 
 
 # Requirements
       Python 3.6
       apt install python, python2
       
 lief installation
        
       pip install lief
 
 xtract installation:
        
       pip install xtract
 
 ## INSTALLATION
 ###     Termux,Linux & Windows
 
 Not checked on MacOS
  
          pkg update, upgrade
          apt up -y && apt update
          pip install lief
          pip install xtract
          wget https://github.com/AbhiTheModder/frida_injection/releases/download/release-v1.1/frida_injection.py
 
 Now run frida_injection.py
          
       
# USAGE
 
     python frida_injection.py
     
## NOTE
 Now you'll think why i made this as a new repo ?
       The reason is simple that Jorge stopped the work and furthur improvements on it and i'm a believer of non-root so i thought to continue this project....😊😊
 
 
 
 ## IMPROVEMENTS
 
 Pull requests & issues are always welcomed 
 
 
 ## Video
 
 Video by <a href="https://twitter.com/leonishan_">Jorge Lajara</a> 
 
 [![asciicast](https://asciinema.org/a/HEz43ylizrdbnYy1nchZ2Hdq6.svg)](https://asciinema.org/a/HEz43ylizrdbnYy1nchZ2Hdq6)
