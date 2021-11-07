# SquidNet2
```
                                  /\
                                 //\\
                                //__\\
                               //____\\
                               \\____//
                                \\__//
                                [|__|]
                                [|__|]
                                [|__|]
                                [|__|]
                                [|__|]
                                [|__|]
                                [|__|]
                     /)         [|__|]        (\
                    //\_________[|__|]________/\\
                    ))__________||__||_________((
                   <_/         [  \/  ]        \_>
                               || || ||
                               || || ||
                               || || ||
                               || || ||
                               || || ||
                               || || ||
  _________            .__    .||_||_||__          __  ________     
 /   _____/ ________ __|__| __|||/\      \   _____/  |_\_____  \  
 \_____  \ / ____/  |  \  |/ __ | /   |   \_/ __ \   __\/  ____/  
 /        < <_|  |  |  /  / /_/ |/    |    \  ___/|  | /       \   
/_______  /\__   |____/|__\____ |\____|__  /\___  >__| \_______ \  
        \/    |__|             \/ || ||  \/     \/             \/  
                               || || ||
                               || || ||
                               || || ||
                               || || ||
                               || || ||
                               || || ||
                               \\ || //
                                \\||//
                                 \\//
                             ____-\/-____
                                 -__-
                                /    \
```
The sequel to SquidNet. It has many of the previous features that were in the original script, however a lot of the functions that do not serve much functionality have been removed.

# Disclaimer
If there are any damages done by this script and are not caused by me directly, I will not be responisble for any damages caused by this script. This script was made for educational purposes only. Thank you for your understanding.

# Main Features:
* Remote access connection  - Control the bots when they connect to the botnet.
* BotNet Admin              - The one and only account on the server that can control the bots.
* FTP Possiblites           - Files can be extracted from the bots into the server directory, where the admin can extract the files inside of that directory.
* DDoS Attacks              - Conduct DDoS Attacks using the bots that you have in your fingertips. Make sure to have permission from the domain you are attacking!
* Config File               - It is rather inconvinient to constantly have to enter the information with option parsing, so instead a config file can save you from all of that trouble.
* Ransomware in bots        - A ransomware script(basically an upgraded RansomSquid Script) is inside of the bots, where it will be activated on command.
* Keylogging                - The ability of keystroke logging is in the bot script, and can be activated or deactivated at will.
* Logging                   - Everything on the server is logged(except for the passwords), including errors and connections.
* Focusing Connections      - Focus on one bot at a time, if that is needed.
* More Optimised            - The script is more optimized, so that it is less likely to slow down or accumalate errors like the original.
* Logic From DatCord        - A lot of the functions use the same logic from DatCord, so that the script is as optimized and efficient as it can be.

# Remote Access Connection
This BotNet has remote access capabilites, so that Bots are able to connect to the server and be remotely controlled there. There, many of the built-in commands that the Bot script has can be run remotely. Shell commands can also be run remotely, where you simply have to input the command you want to use and it will be run on the bots. There are many things that you could do on the bots, where one of them include the ability to do DDoS Attacks. Similarly to the original SquidNet script, you can do UDP, TCP and HTTP DDoS Attacks. These will not be explained here, although in a different section they will. The SSH Botnet is not on this script, as there were many internal problems that slowed down the script if an SSH Bot were to disconnect, so I chose only to revolve around the main part of it. There are however many other functions and commands that can be run on the bots, where the possibilites are endless.

Server Help Message(As Of v3.0):
```
[(SERVER)]: Info about each command:
[+] Utilities:
[+] !whitelistip <ip>                        - Adds an IP to the whitelist, allowing them to connect to the server during a DDoS Attack.
[+] !unwhitelistip <ip>                      - Removes an IP from the whitelist.
[+] !banip <ip>                              - Bans an IP from the server, therefore having them kicked every time they try to connect to the server.
[+] !unbanip <ip>                            - Removes an IP from the server.
[+] !focusconn <botname>                     - Only be able to send or see messages from a single bot.
[+] !stopfocus                               - Stops focus mode.
[+] !getipwhitelist                          - Obtains the list of the IP Addresses in the Whitelist.
[+] !getipbanlist                            - Obtains the list of the IP Addresses in the Banlist.
[+] !getbotinfo                              - Displays information from each of the bots.
[+] !help                                    - Displays this message.
[+] !startftp                                - Start file transfer protocol between the admin and the server(to get any transferred Bot Files).
[+] !togglelisten                            - Toggles the setting for the server to listen for connections or not.
[+] Bot Commands:                
[+] !filedownload <file>                     - Download a file on a single bot computer(requires focus mode).
[+] !download <file> <link>                  - Make the bot download a file from the internet.
[+] !mkdir <dir>                             - Create a folder inside of the bots working directory.
[+] !delfolder <dir>                         - Remove a folder inside of the bots working directory.
[+] !createfile <filename>                   - Create a file in the bots.
[+] !delfile <filename>                      - Delete a file in the bots.
[+] !encfile <filename>                      - Encrypt a file inside of the bots.
[+] !decrypt <filename>                      - Decrypt a file that has been encrypted.
[+] !open <filename>                         - Open a file inside of the bots working directory.
[+] !viewfilecontent <file>                  - View the contents of a file in the bots directory.
[+] !writefile <filename>                    - Open and write inside of a file inside of the bots.
[+] !sqlconnect <sqlfile>                    - Connect to a Sqlite3 Compatable Database file in the bots.
[+] !changedir <dir>                         - Changes the bots working directory to the one specified(use '%user%' as the user for multiple bots).
[+] !stopsql                                 - Disconnect from the connected Database file.
[+] !stopwrite                               - Close writing mode and return to normal.
[+] !getcwd                                  - Get the current directory of the bots.
[+] !keylog                                  - Activate keylogging to see the bots keystrokes.
[+] !stopkeylog                              - Stops the keylogging.
[+] !listdir                                 - List all of the items in the bots working directory.
[+] !ransomware                              - Activates the ransomware program inside of the bots.
[+] DDoS Attack Commands:
[+] !httpflood <website> <delay>             - Make the bots conduct an HTTP Flood Attack on the specified Website.
[+] !tcpflood <ip> <port> <delay> <pkt_size> - Make the bots concuct a TCP Flood Attack on the specified IP and Port.
[+] !udpflood <ip> <port> <delay> <pkt_size> - Make the bots concuct a UDP Flood Attack on the specified IP and Port.
[+] !stopatk                                 - Stops the current DDoS Attack that is happening(only one can happen at a time).
[+] Note: Any other instructions will be run as shell commands on the remote computers.
```

# BotNet Admin
Like the original script, there is always going to be the BotNet Admin. The credentials of said BotNet admin are inside of the server.config file(config file will be explained later), where you use those on the SquidNet2Admin.py script to log into SquidNet2. There however is only one admin account, and only one session that can be opened. This allows easier ability for focusing connections to one bot, and so that the BotNet is more organized as a whole. The admin account has full control over the Botnet, and can run any of the commands that the bots can run. 

Admin Control on the Botnet(in server logs):
```
[(2021-11-05 15:09:21.240190)][(INFO)]: A new admin session has been created.
[(2021-11-05 15:09:21.246203)][(SERVER)--->(admin)]: Successfully logged into the Botnet. You have access to all of the bots.
[(2021-11-05 15:09:21.251470)][(SERVER)--->(admin)]: Input '!help' if you need more info on the commands.
[(2021-11-05 15:09:21.258235)][(admin)]: Attempting to log into the Admin Account.
[(2021-11-05 15:10:02.579047)][(SERVER)--->(admin)]: Sent the help message.
[(2021-11-05 15:10:02.585479)][(admin)]: !help
[(2021-11-05 15:10:53.549310)][(admin)--->(BOTS)]: o
[(2021-11-05 15:10:53.566584)][(DESKTOP-M0LGMU92)]: 'o' is not recognized as an internal or external command, operable program or batch file.
[(2021-11-05 15:10:57.781446)][(SERVER)--->(admin)]: Activating Keylogger script on the bots(All of the logged keystrokes will be in a txt file with the bot's name).
[(2021-11-05 15:10:57.788647)][(admin)--->(BOTS)]: !keylog
```

# FTP Possibilites
This script has proper FTP capabilites. If you need to extract a file from a bot, you will need to be in focus mode(will be explained later) so that too much traffic isn't sent to the server during a file transfer. This means that only one bot at a time can transfer files to the server. The way a file is extracted is that the Server sends a message to the bot, so that it could then send all of the bytes of the file to the server, will the server will process those bytes into a file with the same name. The filename will be specified by the admin. Once the file is saved on the server, the admin can now extract it. The admin activates FTP Mode(the command is "!startftp"), where there commands will not be run on the main botnet, rather FTP mode is simply recieving files from the Server. There is also a help message for FTP mode(the command is the same, "!help"), where there is info about how to use them and what their use is. The Admin can extract files from the server, and have those files on their computer to save. This does work, as I got one of my friends to download the Bot Script(with them knowing of course), and I extracted their Chrome History(it was luckily clean :) ).

FTP Mode Help Message:
```
[(SERVER)]: Info about each command in FTP Mode.
[+] !help                                    - Displays this message.
[+] !fileinfo                                - Displays all of the files inside of Server's directory.
[+] !download [filename]                     - Downloads a specified file inside of the Server's directory.
[+] !listdir                                 - Gets all of the files inside of the Server's directory.
[+] !stopftp                                 - Return to the Botnet and controlling the bots.
[+] Note: You will be unable to send messages to the bots in FTP Mode. You can return to normal by inputting '!stopftp'.
```

# DDoS Attacks
This Botnet can conduct a few types of attacks. This includes, TCP, UDP and HTTP Flooding. The TCP and UDP flooding is similar, where they constantly create socket connections and flood the target with unusual packets. The HTTP Flood is different, sending HTTP GET headers to the target, with different query strings, user agents(and more) in the header. This can confuse the target server and bring it down. There is strength in numbers, as many bots are more likely to take down a server, rather than just a couple.

TCP Flood DDoS Attack on one of my Servers, with packet size of 1024(Started by SquidNet2):
```
[(('192.168.0.87', 51683))]: b'`\xf5\xabY\xcb\xf1\x94\x92\xc1\x19!\x16\x96J\xabE?\x90x\xa3\x89*y\x99\xa2\'\x19}\xdb\x1e\xa9\xd4?oW\xab\x10\x1f\xd5:\xbd\xab\xf6\xf5\x01\xbf\xee\x19\x06\xdec\x7f\x8b\xd0\x9d\xe6\ro\xe0\xda\r\xdd\x12\x90\xdf\tBdS\xc0F}W\xa7\xeb\xc3\x08\x04/\x7f\x1f_\xb5\xfa\xc3\x8d\xf9\xb8\xad\xb4_A\x93\xff\x01\xbb\x87!%a\x9f\xad\xf0\x868v\xbex\xad\x83\x8eK\x03\xb3\x89\x1b\x07NaN@\xa4\xc1<\xe4\xd4\xe0\x1e\xec\xb3ZN\xbes\xae\x92]\xfe\x98L\x8b\xdb\xba?.P\xeb~\xef\xc1\x9e\x12\xb0\x83u\x1c\x01\x89~!2K%\xc8\xca\xb7X\x87R}\x8b\xe0\xab\x17\x12\xa0\x9a\xc5\xac\x0e\xce\xe9\xf5\xc9K%n\x17k\xa0`(\xef\x7f\x12L9s\xdf\x07\xb0\xaf\x15?\\m,\xe6\x8d\xfd\xc3.OCV)icujWT\xe2t\xe86~2\xb2\xec\xed+\xa0\xbc\xa6\x9e\xc5\x8cX\xbde[\xe3\xda\xa3K\xd7\x17{\xe1\xa9\xf0\xe3dm7\xf8\xdf\xef\x98\xa8n\x92\x8b\x01_\x96\x87\x89\xbb\x0b\x00\xc6$y\xf09$W\xad\x8bs\xb6_d^\xe6\xad\xa4\'\xa6\x85\xfasd\x9f/\xf4\xa3\xf7!CR\x01k\x13\xeb\x96\xa1\xf6\xe8\x0b\x91\x86q\xfe\x0621\x01\xfb\n\xe3d\x9e\xbf\x9f\xe4o\xfb\x14\x1f\x024\x13FeT2\xea\xd4N\xd5R\x1c\xbe\xa5\xc5\xdfBj\xc0 \'Q\x0b\xf1\r\xff\xf9*\x93^{\xcdY\xa6D,\xe6\xb3\xe8\xb34q\xc1\xd6\xe3H\x0c?\xa6-\xc8A\x01\xaa\x831{\n}1\xee\xbc=\xbc\xd0\xf8\x8bO\xe7M\xbf@^\xb8\xa8\xef\xb5\x98\xd7C\xe4(z\xa4\xc2pO\xedhy\xb9H\x89\xee\xee\xba\xd6\x11%%\xfb\x02\xd0.c\xabN\x0f\xa2\x16\x98\x16&\x11J5<?iL\xcbcz\x99\xf7\x13\x9f\xd9\xfc+\xce\x02\x9f\xadM\xd6\xca\xbf\x81\xe6%c\x12\xcf\xf6Djp\xcf*\xec\xc1\x95%\x0fA!\x14\x9c\x0et\x92\xf4\x9a\xe5\x86\'^\xd1\x18\xe2k\xabd\x1d\xf1Pk}\x1d\x0b\xa9c\x94\x98\xbd+\xd0\trc\x88y\xe8\x92\xe8N\xfdb\xb1\xb3:\xfa\x18\x17\xaf\x8f\xb7J\x86\x8bl\x19Tfy\xb0\xc1.\xd7\xf1P\x98\xa0\\>p$\xa2\xc6\xe0\xa3(g!\xce\xacA\x8dP\x87\xa5\xdc\x00\xd7\xf7\xc6\t\x88\xd4\x16\xb2\xb6\x8e*\xeaP\xda\x9eh\xc5\xb2Fwl\xe2\xce3\xf3=\xdd\xac\x95`\xf4\xb0\\\x04\xa4\x11M\xf4\xb1\xc5\xe5\x8a\xa3F\xae\x98\xb8\x12\x06\x9d\xf3G\x08\x86\xee&\xcb\xb6\xb3h\x880\xf1Yt\xb3/n\x18\xaf\xc1\x92\x1e\xcf\xd1\xaf\x0c\xed\xb2\xab\xc4\xdb\x8an\xd8\xef\xa6p\xdbFv\xf7;\xfeo\xb6|\x98\x872\x89\xe8\x8a\xa6z\x0c\xf5\x84c\xfc\tp\xc5\n?\xae\xe7\x17\xc9\xa4\xbe\xd4-\xe7\xf1\x84\xab\x142\nB{jz\xeb=\x13H\xd2F\xfa[$M\x1f\xe8\xd1S3\xf6\xfb;\xb8\xdf\xc9\xcd\xf2\xbaw\r6X\x9b\x17\x02\xb2\x10\xf1x\xc0\xcd`y\xf0\x01\x85\xc0\xb6I\xe2!\xd2\x80Q\x8c\xb5\x80\xe4/%\x8ce\xa8qV\x1bK\x8d\xa5\x81/=,$\xe0\xce\x86\x02\x81\x1e ~\xf9wO\x16\x99\x9c\xa4\xc2\xef\xaf\x88\x01\x93\x8bl\xb2\x7fV1\x14n\x99\x13\x18\xf3\xc3\x88,\x0bS)\xe9xaf\xe9(\x01\xafxkS\xe3j\x95\xd9)bPAl\xa1rh_\xa5\xce\xdb.V\xb5S\x88\xa7\x9e\x8c\xf3b\n\xb4 8\x17\x0e\xe6\xcd\xbd\x19E\xe2}\xa8\xd7\xac=_\x89\x1f2\xe16\xab\xf7\x1c\xca:\x97\xf3n\xff{\xb4r;\x07\xb9bOw\nU3#\x81\x0e\x9d)T!-\xb3\x02\x8d\xbao\x9bTf\xee\x87\xbf\xb7^F#|\x14\x9c\x83v\x17\xad\x99\xc4"o\xe5\xefP\x12\xad\xb0\xd9L\x1f\x11\xf8M\xee\x1d\xdf\xaa.\x1c9U\xf0\x94_bj\x9a\xaa\xdbc\x90=I\x8b\xd4n\x8b5\xe5\xfb\xf3\xe6;\x98\xa3!`\x8a`\xdfA\xff\x06\xca#\xf7\x02\xfc\xfe?V#\x02P\x81D\xd4\xaa\xe9\xddH\x84\x9b3#\xa9>\xb4\xf1\xff\xc03\x83\xc0=\xfcUF\xcbz'
[+] Connection: ('192.168.0.229', 52606)
[+] Connection: ('192.168.0.229', 52605)
[(('192.168.0.229', 52606))]: b'p\xe7\xd3\xb6r\x80\xc0Z\xf4e\x1b\x8e\xa0\xbd\x98\xc8\xee\xd5\x8c\x8d\x03\xe2\x88d\xaf\x9e$u\xe2i\x96*\xe4W\x96\xc7`\xa4e\xae\xc1\xfd\xc0\x7f\xac\xde\x90\xba\xfc\xb6\x1a\xd8\xd9V\xc5v\xfd8$\x8dc.y\xed\x8a\x8d\x07O\xd1\xe2\x07\x88\x17\x1d\x8e\xe9\x9cU0\x19\xac\xa1\xbb\xaf\xe9,\x17\xac\x0f\xc74[\x03\x9c\\5Q\x82\xfb\x80\x1d\x02\xc8\x03\x9a\xe0\xe1<\xad\xf7\xebHd\x04\xc1#x\x95\xfc\x08\xa2\x80\xf1 {h\xf2\x9a\x92Rp\x10\xc3\xab\xbc\xa5Q\x1d\x89\xe2\xdev\x91\xfd@0\x88\xc0Ba\xeeQ\x18\xc3e\x064\xdd\xbb\xd3#@R\xd5\x9e\x7fz\x8f\x06T\x8a\xcd\x99\xc6\xad\xb2=\x12r%\xea0\xace\xa2d\xbe\xa8f\x9f\x90\xd9D\xf8F\x82b\x06@\xeb\x16gw\xc3N\xd7\xb0\xf1\xb8c\x9b\xc1J$\xf6\xca\xd0\xf27\xda\x89nB\xd8\xf7o\xb6?6\xfa\x05,S\xce\xdd"w\xa3\x8c\xb4E\xff\xabZ\xbd\xb6\xeb\x84]\xbf\x15\x82\xf2\xb2\x1d\xf0\x0e\x1bN\xb8\xb1\xfa%;]\xbegE\xed\x152\x9c\x8bH\xe1Y4\x05\xb5\xc7\x10a\xea\xe7\x81\x88s\xf5\xf2\xdf\x8cD\x1c\x06(\xd4oZ\xf3\xd2\xb3c&E^6\xb2\xc7\xfd\x10\xd6\r\xa2J@\xa3m\xa6u\x8d`t\xf1\xf1\xe4\xfd\xecVOOWC\xacx$\t\x82y\xf4A\x05\xef\x7f\xd6(\xa7\x94\xacl\x1cc\xfe\x97\xb6\x95\xcc\x98\xe5{H\x98\xe6\x10\xb8\xdb\x93\x00\x05]\xa9\xab\t\xfc\xe9\xc7\xe4\xb6\x08\xb2_\xf9\x1b\xbfl\xff\xb7[\xc8!\x8e\xb0\xc8\xe2\x85Mu\xe3\x88\xba*\x18\x84\x8a\x81\x96D\x89\xb9b"\\G?$>\xe7\x15\x03S\x9b\xf4\xc6\xc4zu\xcb\x13Oe\xd8_\rsQH\xb9P]\xecUv\x06-\xf3*e\x84\xbb"D\xb9\xc4\xaf\x17z\xc3\x8b>\x02X\xb4\xdf4\x88\xaa7\x9fy\xbaC[\xdc7c(7*?\xbc?\x1d\x071\xc7\x90\x13\x84p\x18\x0b-\\\xa7\x130\x0e\xb3\x0bu/\xba\xb0\xf8\xce\x85\x1a/\xe8\xc3\xb7\xcbl\x86\xcb\x99\x900\x16/)J&\xe2\x95{]\xe4U\xe9K\xf7\x13\xbb\xc1\xb2e>M\xf9\x94#_\x8f\xed\xc2x\xc6\x9da2\x8b\xc6\xcc\x00X\x1f\x89*(%\xfd\x05\x1f\xd3mP-\x15\x8fD\x17\n\x9e\xee\xd5\xdbZfi][\xb3V_L~U\x9cM\x0e\xf1\xc8-H:\r\xd95\x8ae\'\x9a\x11\xc8\x1bL\xf2\xc4\xd3\x13\xd6\xa4f\x06A\xccTW\xf8\xe6rd\x82\xf5\xc1\x90\xdd\x9a1\xc8\xec\x04c\xcc=\xb4\xcd9TE\xc2>\x83EsS:sd\xc39T\xd7\xe4\x0c\xba\xa1|\xb2\xd4\xd5lo\xbc\xe0\xd2H\x9d\xd9L\x16\x14\xe1\x96*v\x1a\x13\x97\xa0\x0c\xd4,\xb4O\x11\xdctB\xe9\xb0Bw\xa6r\x89qB\x8e\xfe\x10\x89\x18B/C\x13y\xbbU\x16\xd1+g\xcd\xffZ\xb8\x9c\xbc\xc2XB\xff\xef\xb3\xda\x9a;"5\xfcw\x11\rfw\x9b\xc4\x7f\xb8\x17?\x9a\x00\xe9;\xfa\x8b\xe7\x91/\xd7\x1fM-\xbe\xa4\x14G\x95\xb0s\xc4|;S3\x11d\x8c\xc2\xbbA*;\x12\x14L\xa7\xcb\xa0p\x15\x10\xce\x97\x9c\x9f\xc1\xbew\xc2$!\xe5\xaf^>C\xf8\x99<C\xb9\xd4\xa3F\xafF\xe6;\xc4\x89\x9a\xd8\xe32Qp\x19\x02M{\x13\xa6/\xd0T!%?K\t\x8d\xfb{\xfb\xf3m\x9a\\\xfa-\xa84S\xc1\xec?9\x7f\xa6\xb8\xf2\xa3\xf5V\xf2\xd6E\x1c\xdfD]ig{\xd6\xf9\xb8\xa6x\xc7\r\x80\x04M\x90Z\xd1\xf1d\x11M\x90\xae\x19!>\x03\x90\xab(\t4\xeb\xfbA\xbe\xc5\xf0\xb9\xfb</\xbcLZ\xf1\x02\xc8\xde\x08\xc0\x0e\xfe7\x8e\x009\xae\x05\xed\x8f\x1d\xe8\xae[\xe7\xa7C~\x92\xfd^\xb8m)\xa0h+c\x1a\xb2$#K4\xb8\x01>\xfd\xc8\xfe\xe5\x08.\xab\xa7\x15A\x016\x98\x8f\x14j\xb1\x0f\x8b\xaf}\xdf\x04\x0e\x9b3\x7f\xc1\x9e\xdf\xd5W\xf5\x83\x9e\x92ng\xdfY\xa7\x83\x1f/f\xa9Rs\xd6W][\xa6\xbah~\xfeIf\xcf\xb0\x02\xbaD\xfbU\x93\xa2\xe4z\xb1\x07'
[(('192.168.0.229', 52605))]: b'\x94\xf3\x04\xab\xf3\x02\xc3\xd4u,{0L\xbaf\xa3L\x838Q\x02\xc5\xbb8\x00w\xef\xcdq\x99\x15\x98\xcb_\x12\x16\xa3\xf5\xb65|)\xde\x8d\x8aNV\xa3\xc1;99\x82f\xf9\x19\x16\xa8\x9cR\xa4\xa6\xb1\n\x14\x04\xeb\xe5\xdc\x1e\xcf\x10i\x06fw\xf45\x97)\x89\xae 2\xfd\xc0\x1bI\x91\xe8%D\x06\xa5P\xabF\x9c\x13\r\xa9\xcd\xf6_\xd27,\x0c\xac\xe1\xb71\x82\xd2\x96\xe9\x1f\x0ed;:(\x0b\xfc\x03/t\x02\x1a1\x8c\xb8p\xb9\tor\xf1#\xfb\xd9\'\x9bW\\d\n\x8f\x1e\x87\xa7\x19@4\x99\xfe\x88e\x01hC\xf6^\xf9Zb[\x95\xa4\xd4\x89yym)\xa0\xea\t4\x0bJ\xba\x85|\xf8\xb2\x9a,\xca}\x96\xb7\xd5\x9b\x90\xac\xb0\x8a\xacyk\xaa\x84\xc2\xa4\xb71o\x1f\xb9+\x9a\xbc\xaf<\x86\xbf\x17\x06\xac\x92\x8e\x81\xb2G \x90\x9ac\xbc\xc8\x82\x02:eb\x9b\x011\x8d\x90\\B\x8a\x9bX\x88\x1f\xfci\xdfJO\r\x7f\xf2YD\x9dU=\x8f\xeb\x96\xf4\xb7\x86\x02\xc9\x02p\xc7L\xa0\xa5\xe4\xef\xea\xb06\x91\xa4g\xae\x18\xd7p>\x8c`\xb32\xa4\xd4\xe8b\xcc\x82\x99\x1d\xa1\xdc\x9bv<\xe3l+\xd4 \xff\x14+\x06&\xc9[\x1bs\x86\xf5\xb9\x176\xdd\x9c&\xe3G b\x9e2T\xf0\xa2\x83\x04\xf1\xed6L2`\xb9\x01\x14g0\x9b\xbc\x87\x01Q|{\xdf\x163\xa4Z\xf1/\x8e\x0fz\x86\x86\x14\xe4\xbb"I\x0c\xea\xca\xd9\x87G\xe9[<i\x17eC\x03\xbf\x87u\xab0\rKGp=\xfb\x01A\xe7\xa9k\x97\xb8P\x0b\xeb"\xf4\x01\xc5\xf8\xc6\x94\x0c/T\xfbB\x98\x02u\xd4\x1e\x8f\x8e)!x\xd4\n\x1d\x02_+\xf7\xf4^T\xce+\x1e\t\xa2\x87\xc9y\xe8\xc1\x1axd\xb15\x87\xbdx\xb3\x8c\x81|\xce\x90\xf7 U\xa1;\xec\xb7]\xac\xe4\xec\xa4/9I\xd5uJVti\xce\x03\xb3\xe5>\xdd\xf82\x9a\x8a\xb8\x18\xd0\xdb\x94\x8c0\xd0\xc6\xba\xc1\x1bV#\xc8/I\x18\xa4>*\xb3B\xf8\xf4\xef\x89\xc5s\x85\x88TQ\x13\x1b\xc1\xf7`T,`\x88\x82\xad\xbbP\x92\x1b\xa1\x079 \xc9@b\'\x983"\x98=\x8e\x8d\xafeO\x1e\x97\xef\xb7A|\xd7b\xa2\xd3\xfaP\x7f7\x7f\xde4\xc2L\xe2o\xb7\x1f \xe5r\xe3\xea\x89\x1f\xa8\x9b\x0b\x12\x93\x1e\x06\xee\xeab\xee\xda\xc2P\xabk\x80\xa4\x93j\x98\x04\xc1@\xb99iKX\x1b\xe4B@\n\xb2\x1a\xac\xc5"\xb2=\x1fc\xee\x8a\x94\x0cb\x00\xfe(\xa2I\x1e\r\x1f/\x08\x0ct\x05\xddzA/n\xe6\x8a\xe7\x9e\x1c\x18\xea\x1a$\xaa\xa6\xb1\x8eZ\xe8\x86\xff\xec\xaf\x94\xa2\xacf%\xf0\xe2\x97E\xaf<\x1c\xd3\xb2\xaa\x81\x11\x85\x19\xcb\xd5D\xeb\x183/\x8a,\xa7\xbaxxger\x96B\xe6\x97\x90\xd7-\xd0\x8f\xf1i\x00\xbf\xbf\x18\x1b\xa9\xd1\xed;f\x99M4\xf8%\xe0\xd5\x11\xc3S\x04\xdc\xc0\x9e\xba\x13\xe6I\x9bOz\xbcY2\xb8\xc2\xc0\x1dX\xfd\xeak~\xac\x02\xa5m\xd6\xed\\\xd6\xbc\xaeu\xdd1_6\xc4\x04v\xceY\x9c\x05\xf2a\xc8\xc8\x07\xb2\xfc\x06\x17\x92zi\xcf\xa9\xdev\xcc-\x17\t\x05\xd6EjOP=H+\x9e\xc3v\xfe\xd5>\xef\xe0@\xa6\x8d\xb5K\xf9?\xe5\xca\xf8KC\xa6[\xa4\xe0\x1eF\x0bf@\xf1\x14\x8b\x82\x10\xaa\x1d\x16\xf1?\x8e&\x93?e\x10\x85\xfa\x02#Me\xef\xa8\x1b`\xda\x92\xe7\xc3\xd9\xe9\x00ZNP\x95\xebM\x1bt\xdb\xc7R\xa1\xd8\x08\xac\xa7J\xed\xe8\x82\xb5\x9d\x85/\xf3\x90\xed\xe6\xc4\xf6\xd3\x07\xae\xe9\xba\x95\xbf\xdd\xd1\xa5b\x13\xb7RK\tYf\x88\xfcH&\xf5\x00*Q\xdf>\x86\xa8\x840\x82\t\'QA\xecc\xd1)M\xe8\xe7lm\xb1P}\xe9G\xecL\xf6J\xfdj\xc5\x04\xcb\xa1\xc8\xe7Q\xbc\xf8\x98>9D\xc9:\x93_cG\xd6\x03\x94\x85t\xca\xb7\xeaq\xbe\x9e\xfcY\xef\xd1\x9c=\x93E\x18\xbb\xf4\xbe\xd6\xddw\xc3\xa1\xf6\xb3\xb2\xd1#O\xa2w\x9d\xbb\x12v'
[+] Connection: ('192.168.0.229', 52604)
[+] Connection: ('192.168.0.229', 52603)
[(('192.168.0.229', 52604))]: b'i\xf9\xb8c|I\x04\x91h\xe0\xca%\xbd\x00\xf0;\x9fl\x98"\xf5f\xcf\xe0\xea6\xe5\xbd\xf9\x9d\xbe\xe6\ro\x0fY\xacg\xbb\'\xf4X\x06\xb0\x81\xa8\x05\x1ba\x81\xa9\xaf\xfd\xf2zDaE\xf0\x84\x8a\xbf\xad!\xcc\xac\xd6\xf1Z\x08b\x9d&\xf2\x1f\x023\x18\xc0\xc4\xe0V\xdeV\xa7gI5\x17\xf1n%DxR\xcc\xb7@\xe0\xc3j/\xba)k\x96\xb0\x8aZ\x87\xf4\xc3\x0e\x96\xa5\x8a\xfa(\x9ay\x1b\xca3*9\'p\xb9Fi\xf5\xd1\x1f"\x8d\x95N\x7f?p\xd1\xe0\xb9v9@ \x17\x81\xc5\xf8r\xe9\xb8(\xaa-\xd2\x9c\x94\xd3\xfe\x07j\xf7\xaco\x11@\xfd\xb0\xf3\x1d\xa3$\xa9(&I\x1fV\xecUX\xd1\x18\x0e\x0b\xfa\n\xfe\xf9Z\xd1\x03\xb2\xa9\xfb\xbd\xe7\x8d\xb8\xb0\n>a\xa3\x8d \xab\x8c0o\x07\xdcY\x83\xf1h>;KxV\xca\xa7\xa5\x11-\xcfR\xdbn\xca\xc5\xfc\xc6\x10\xff\xc9\xa4a\x84e\xe7YM\xbfD\x19\x08\xa7\x14\xdcDg\xda\x86\xab\xd1\x9d\xa4]"\xc0kT\xd9A\x0c! \xe5\x8f\x04w\x9b\xc5,\x12\x05ZOHH\xb2\xe37\xc9@\xc2\xd3\xbf\xee\xa9eY\xaa~^\xd6\x83+\x0eW\xdft\xd2\x1eq\xcdq>\xfd\xd2\x9e\xd6[\xc7z:\xac\x1c\xaa\x843P\xde1jS\xfe:\xf8\xb9l\xa8x\'\x03\x9c\xd7\xbevx\xc1j\xd6gK\xcfEu\x87fy\xfa\x05\x04\xc1\xeen8\xc6hT]\x9a\x90\x1d\x8b\xf8r)\xda\xa9\x10\xf0x\xd9\xfb\x19\xf6\r\xdbJ\x80\xc2\xdbf,\xc0Y\xae\x00\xd8\xe7=\x9b\x16\xc5e\x1a\xecxL6s\xf20\x985\x87\x00;\xcf\xab\x1e\xfb\xa9\xc9t\xe5\xcd\xce\xa8\r\x94t\x912\xd0<F\xe9\xe0\xbe\x94`\x85\xb8\xa2\x8f\xbe\xa2\xb7\xf0N\x84\xe8\xc5\tK\xac\x9e\xf3\xcd\x8b\xd0\x9bi\xcd\xcd\x83\x0e\xa2{7\xa0I\xf30\xdc\xb1\xce\x9f=1@\xf2:\xcbP7D\x91ppY\xbb\xcb\x12\xee\x1d\xce \xc9\xa7y;\xb1)v&\xd2\x8c]\xa1\xba\x9c\x89\xf36\xbe\xbf(5*a\x07\x849/\xdey\xdc\xc2rp\xc9\xf8\xb3\xfb\r\x89\xf5\x0fy\xa0\xb2\x1d\x9c\x81u)\xa5\\A.CQ\x840\xc2\x87\xea\xb2\\r\x89\x80?\x14\x98\x0b\xa1^\xa9\xe8K\xeaA\x1f\x10\xf7\n\x94-\xfa\x95\x11\xd2\xdbC\xa9(\x94Qn\xf9\x1ey^\xc3\x0f\x10\xea\x80\xd5\xf8\xc1[=\xb5\xa3\xe4\xbf\xb3\xb2\x05}\x91v\x1522w\x90\xc4\x83\xc3 \x96\xfa\x19r\x8e\x92\xca\xe12\x9cM\xbe\xdf\x8a\x87.7\xb7\xce\x0eq\xbf\xf7\x87,\x8d\xe1\xebiL<\xe3\xe64\x1c\x8d\x0bb\x9c\x14\xa5[L"^_=\x16kY{w\xe8\'\xcc`$5VF\x08Yux\xa6\xfc\xb7YS##M\x85\x11Mw\x08\xa4u\x93\xa9Jc\xe3Oq\x01\xb1&&\x82\x8c\x95\x174\\-\xf4\xb3\xf56\xba\xe4]\xa4\xb6\x1c\xac7\xb3\x92<e\xce^OF\x0ep\xd7\xaf\x8b\xb7H\xfe\xc5o\x0f\xf1/<d\x9ff\xc2[\x07\x92\xd5e\'\x91\xc4\x00\x7f\x16[\xc2hZ\xe3\xfcc\x7f\x81\x10\xa4\xd1\xc9\x98y\xbb\xbd\xe0X.\x90\xc7\xd2\xe8\x0e6\x88\xd7\xd9\x92\xc3$f\\l\x983\x0f[\x91\x18\x9ec\x1bV\xf5\xdb\xe3c\xcc\x7f.\x9f\xe6\xcf\x08o\x1f\x91\\iN,\xb2\xd2\x99C-\xf46\xdf[\x8f\xf1^\xf8\xe1\x08\xa2\xcf\x90\xdf\x02r1\xde\xe6\xf4z@\x99\x00\x8at\x9a\xc4!\xa1j\x96\xeb\xd9\xb0Q\xea\xc4\xf8\'\xb3\xec\x0b\xb7\x08t5\x83\x8cnr\xff\xb5w\xb5(;\x13\x14\xd4p\xa0\xbbx#\x0b \xd8\xc0\xfe\x15\xee\x8b\x96u\xa7!{\xcb\xc8\x03#>\xc2\x90$\x12\x94\xfc\x80\xf2!\nb)\xe83]\xff\x01-\x04\xe7\xc1\x82\xc1\x7f\r\xcdi`\x90\xe8u\xf8\xed\r\xbehIr0\xae\x82S\xcd\x81\xaa\xd81uP\xc9\xe6\xe2\x1eC>.\xd58\x03"\xcc\xfb\xb6r"\x84\x14\x84\x08\x1a\x16\x88\xe4$\r\x1br\xfb_9\x17\n\xf7O\xa2N\x82\xa4@T<^K8\x94t^ \xff\xac\x97\x12\x1ez\x9c'
```
HTTP Flood on one of my Webservers:
```
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63790) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63789) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63788) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63792) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 56983) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63791) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 64960) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 56986) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 64961) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63795) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63794) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 56990) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 56993) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 56995) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 56996) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57002) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57003) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57006) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57011) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57012) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57015) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57019) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.87 - ('192.168.0.87', 57021) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63793) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63798) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
[+] Connection: 192.168.0.229 - ('192.168.0.229', 63797) ---> 192.168.0.87:80/ - HTTP/1.0 301 Redirect
```

# Config File
I decided to go this route, as Option-Parsing is over complicated if you simply want to run a BotNet. You simply put all of the desired settings and credentials into the config file if you need to. Otherwise, there are default settings that will will be reverted to if there is an error with it. In the config file, you can change what IP and Port the server is hosted on, and also many different settings. This file will be auto-generated in the Server directory on the first time that the script is ran, and you can change the settings if you want to.

Default Settings of the Config File:
```
hostip = localhost
hostport = 8080
external_host = localhost
external_port = 8080
logfile = log.txt
admin_name = admin
admin_password = adminpassword12345
enc_key = iC0g4NM4xy5JrIbRV-8cZSVgFfQioUX8eTVGYRhWlF8=
ftp_dir = Bot_Files
ransomware_active = f
```

# Ransomware in the Bots
There is a ransomware payload inside of the bot scripts. This can be activated at any time, but of course on command. This is so that the owner of the bot computer would not know if they have been hacked or not, rather the payload would be used only if it is needed. The ransomware script uses the same encryption key(specified in the config file), and will use that to encrypt its files. What the payload will do is encrypt all of the victim's personal files, so that they cannot be accessed properly. There is of course a way to reverse it, as in the %USERPROFILE%(This is for windows, although other devices it is '/') directory, where there is a key file that can be accessed, and the actual encryption key can be placed inside of there. The bot script constantly checks whether the correct encryption key is in there or not, and if it is it will decrypt any of the encrypted files.

Non-Encrypted File:
```
We're no strangers to love
You know the rules and so do I
A full commitment's what I'm thinking of
You wouldn't get this from any other guy
I just wanna tell you how I'm feeling
Gotta make you understand
Never gonna give you up
Never gonna let you down
Never gonna run around and desert you
Never gonna make you cry
Never gonna say goodbye
Never gonna tell a lie and hurt you
We've known each other for so long
Your heart's been aching but you're too shy to say it
Inside we both know what's been going on
We know the game and we're gonna play it
And if you ask me how I'm feeling
Don't tell me you're too blind to see
Never gonna give you up
Never gonna let you down
Never gonna run around and desert you
Never gonna make you cry
Never gonna say goodbye
Never gonna tell a lie and hurt you
Never gonna give you up
Never gonna let you down
Never gonna run around and desert you
Never gonna make you cry
Never gonna say goodbye
Never gonna tell a lie and hurt you
Never gonna give, never gonna give
(Give you up)
We've known each other for so long
Your heart's been aching but you're too shy to say it
Inside we both know what's been going on
We know the game and we're gonna play it
I just wanna tell you how I'm feeling
Gotta make you understand
Never gonna give you up
Never gonna let you down
Never gonna run around and desert you
Never gonna make you cry
Never gonna say goodbye
Never gonna tell a lie and hurt you
Never gonna give you up
Never gonna let you down
Never gonna run around and desert you
Never gonna make you cry
Never gonna say goodbye
Never gonna tell a lie and hurt you
Never gonna give you up
Never gonna let you down
Never gonna run around and desert you
Never gonna make you cry
Never gonna say goodbye
```
Encrypted File:
```
gAAAAABhhty5_0NNHt8_3DoW_3qdYH93yew1fjlUD1K50GjRfGoQkwm1ZSBco1DrCPnmJXMc8Ojq6gqwisMGHVfcYS-AYsuYpKvNNz008-IwJUmNo0IP6GMnb4eH2UsqZ8dqCZ9_3DVNojdUt_A3lnI21P7reF75BAR18M3ed7_1ehyZPxxdxuMchsvzvmuZw6V1BKlsx6Jd9JyNar-MvE1_uzjOEDV_gpGIJ_P1pTOPmEOD5WOUAKGIcMWW0XHYMeGag2dmiznqOhg5pDJ_R-ZV9MzBnBNniefD3LhLLDJ-d-ipFGrk0IpeU2uPHPGJRmzrPyg_xHko9fOs3OfcIzpZ1fgLq1m-sfg-bTJSoBPhx1Z5qEjRA7gnZOK6aJp_vIECffbeev36nf2pc8bD7BqaWYUTX6BHz7k4it2CPoAsqh4osAvhrI_2kq2Pw2r5rdFsGqGc-q-UBgk1hHe46TkX0jqgC_VWM9ZTSinivan0mXdmgwp6ghfTHt-7BfebCWMwDOj6p93wfyIzM5HqSXbUw4UUoRDlFRpofdtCoivKzVN7yHmR2RudX46YXhwcl2hXBmApIxRI__QufCa9LnqgIy1PDUfd45qNqX4ocZ4ZlSAz4onOcSgQqtVqYukfWooNiSAD_Ar3vvHQm1BjjU6CRiGgS81hJred5BxzH__yTsPQSNLUrMcDAONQQsRYvWbuci7NGLWH82FtCBivrlDIUAnXdeNFko1MGLUCzg64xir48Gzii5brrWG3vo8QeZewHZTgjSSW_Pd99AaQa6mHFw29RhN3SjXQr964kMBD3UlveZh7DO0fFNc9RdbTpUO_mM3ZdUo3m8ihw2-BxTJmFbkB30XM4oL_AFpHFnT5GonLV1YHqf3Est7Gg4hvO-yfex9LWKxAHwO0rCUnw1MZZcKJtEEu2ij4HIqqVBkrUr18TQWnxsn7HTXaqtRr0OuU-J8mHtgzs4zlSeZvd7mLZShaf8oVvcx6wVph7d9twAqiT1J81tvzmIiNLPBzBqtsDMvFZHoHo-zf2OPZpAii9pbacuBW5D9Kv8I0mIVIoHwnDFPcFZSfNIq3b4_z2hW3bzK96lqQnkXX3nb1mSNKLa7TCrbvgdmTmzdFuonFUL3tN354KVuzcRmaClTx1flGAaDwnRvCx9-eoqyW3LTF80Ex-7uqfVjFN6eotpapLnaUdQKePT6aXGbVIPCLyV5Npqr4UWUtAsXiqoVKwzacsMpNt9PBKI2mguo33a7_8okYrheGEtufPW0kf0oEINhOA4Dhqwp5iwVOFwpJAGshK8kikkb0icCY2xxCnpcgHh7xyGIpoClc074lMRw9pUBTZDHyWCOnx0F-gMMRgEADX0oxAMIYXfMggcJth2Uv8lQYiU1yl7KjEFW9f6f8ax4II06omt7iL4L2S-lITeFpTDpzMHiZmoUlZsejqvFMllferoAwplwawVxsxDM1lftudisHkitctnf6R_prEVt7gJM8nP9RMBCk7QerNptkyolY8GZ2bQhOvB8qYdet_Srup-BhzVgz0EuQ_xxVG3YxeqMVSJ2ly8aclAP9FhqeOtnaKVKR-7S6TKvGg2kX87ibHrTNiXkoGJeFk2arfWbYiDM5K0fJvy5WfkNxE4eSIqzQRhh3Tj_8aluVCKW4J9o1F2PTDwX-oYF8JDGbwcQZw0Vuv4h9vEOw-6abwzJFex0kKP0qU7hwQnIWETInV9N8qWIfEByMTKGCcBNIEMJBlVmk-fDbWsbS-Ox3xOVzyRUizrVZvC8Rx-3tSdjcsbCzRYLDcwyZbUdyD7p7D33T4pauRY8UJmgUtGkpq639UU9o6AKqOEcSkzXz6fSsXSYmEaVMrZEVawiKyyjO25HYrcoo_fTDeiEtfEGyvhNr9Ulm8dEDfeVvBpdZJf2eapt7Xp09xrzRlaY29fY1L-oRN4ScepIigz4j__fmm8yGuoZHXqtFLp2ZTezAU8mpy3T2W6BjxnnVCrZzkijCIDm2QpqMRtGIFDKBHu-ZrUiwLSSFIMEuJr1OAQ-twBf1HWBeV8w-nZj3C8vNhp4ZHU5_BVRzs2E-de1BcqTYyofRXV3jyXd8jHdEe_c9Wg9FjZgVm46l7QJarIat5yvDfYj9GSK4cexJCrXBw3H8UmB286I5UyF1yeT74hz5UWGY6yBpSD2lqCzMpWR93IWVzIKPdu8pVs0haVkMlePiSrYmMLmZiF3F_AX73MMTVA_igzX5BwSAlNwK7lpyEVQOpNS5YJ8SP1JujWPdHhp35Puf7itgP0TSojFAF8B2RDW-EpHqbJe-ESp9-rsuQjVfeeJtA0EoA2BNLlJmSvvzj6cwvdui0NCMSCBX4-k7mgTXLNJtDayWArZI-XeCWEb1MTCaOlhxn3UgqjK6itWnuFonDI82hezmnGAJD8qwyzBsXGC2tEP2jVUStqh8Nn_qLWXty7zuNTb8cA==
```

# Keylogging
This is so that the keystrokes of the bots can be monitored. This can be used to spy on what the victim is doing. Whether to be spying on a conversation(of course one-sided), or getting a password being typed into a login page, or even just them gaming(Lots of 'WASD' keystrokes).

Example Of the Keylogging:
```
LOGGED KEYSTROKES FOR BOT DESKTOP-M0LGMU92

[+] 'a'
[+] 'a'
[+] 'a'
[+] 'a'
[+] 'j'
[+] 's'
[+] 'j'
[+] 'k'
[+] 'l'
[+] 's'
[+] 'd'
[+] 'j'
[+] 'f'
[+] 'l'
[+] 's'
[+] 'd'
[+] 'j'
[+] 'f'
[+] 's'
[+] 'j'
[+] 'd'
[+] 'j'
[+] 'f'
```

# Logging 
Everything in this server is logged. This includes every connection, message and error in the server will be logged. There is a log file in the server, that can be accessed whenever needed. You are able to see any of the issues or errors that the server is encountering. It also allows you to send me any errors in the server that could be identified and debugged. Additionally, you can see the log live, as almost everything logged is also displayed on the server script.

Sample of Server Logging:
```
[(2021-11-06 20:32:08.271470)][(INFO)]: Server Started on 192.168.0.87:8080
[(2021-11-06 20:32:08.271470)][(INFO)]: Bots/Admins will connect to: 192.168.0.87:8080
[(2021-11-06 20:32:08.271470)][(INFO)]: Payload Bot Script Generated in C:\Users\pfang\Desktop\SquidNet2\SquidNetServer\SquidBot.py
[(2021-11-06 20:32:08.284802)][(SERVER)]: Payload file has been transferred to the FTP directory(for extraction of Admin).
[(2021-11-06 20:32:08.291071)][(LISTEN)]: Server is listening.....
[(2021-11-06 20:32:09.307653)][(ANTI_DDOS)]: Setting 'self.auto_ban' variable to: False
[(2021-11-06 20:32:45.839599)][(INFO)]: A new admin session has been created.
[(2021-11-06 20:32:45.840362)][(SERVER)--->(admin)]: Successfully logged into the Botnet. You have access to all of the bots.
[(2021-11-06 20:32:45.846462)][(SERVER)--->(admin)]: Input '!help' if you need more info on the commands.
[(2021-11-06 20:32:45.852564)][(admin)]: Attempting to log into the Admin Account.
[(2021-11-06 20:32:51.089415)][(SERVER)--->(admin)]: Sent the help message.
[(2021-11-06 22:35:16.298690)][(ERROR)]: Closing connection with admin due to error: [WinError 10054] An existing connection was forcibly closed by the remote host
[(2021-11-06 22:35:16.312652)][(INFO)]: The admin has left the Botnet.
```

# Focusing Connections
This allows you to take control of a single bot, if you have multiple bots connected to the Botnet. You can select the bot that you want to only see command output from(providing the name of the bot), and you would then be able to send messages to that specific bot. You will be able to extract files from that bot, and then be able to obtain them remotely. You could also simply enter the commands you want only to run on the selected bot, whether it be the Ransomware script or really any of them at all.

Instructions Sending from 2 Bots to Only 1:
```
[+] Enter your msg: echo hello
[(DESKTOP-BVT29KJ4)]: hello
[(DESKTOP-M0LGMU95)]: hello
[+] Enter your msg: !focusconn DESKTOP-BVT29KJ4
[(SERVER)]: You can now only see output from bot DESKTOP-BVT29KJ4.
[+] Enter your msg: echo hello
[(DESKTOP-BVT29KJ4)]: hello
```

# How to Use(For beginners)
(Coming soon)

# Overall
SquidNet2 is the sequel and superior version of the original SquidNet. While without some of the original commands, the functions and functionality of the new SquidNet have been improved on along with the new features added to it that help with its usability. 

# Happy (Ethical)Hacking, DrSquidX
