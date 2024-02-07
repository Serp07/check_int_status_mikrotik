# check_int_status_mikrotik

This script monitors the state of the VPN interface (but you can add other interfaces), checks it with the previous result in the file and, if necessary, sends a message to Telegram.




local iFaceNameFile "int.txt"  - is a local file from which the interface will be read for further use. 

local iFaceName "your interface" - here you need to enter the interface that we need to monitor.

local previousStatusFile "previousStatus.txt" - this file will store the current port/interface status

global telegramBotToken "BOT_TOKEN" - you need to specify the token of your bot.

global telegramChatID "your chat id" - you need to specify your chat id.



#[/file print file=int.txt] - when using the script for the first time, you need to uncomment this line to create a file on the Mikrotik disk. After creating the file, you need to comment the line.

#[/file print file=previousStatus.txt] - when using the script for the first time, you need to uncomment this line to create a file on the Mikrotik disk. After creating the file, you need to comment the line.
