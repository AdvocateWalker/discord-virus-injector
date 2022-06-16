# Discord Anti-virus Trigger Generator
this script allows you to inject vbscript code that triggers windows defender in images/gif/videos to troll people on Discord

## How does it works???
Quick tutorial on how antiviruses work.
most of vbscript syntaxes that makes GET or POST requests throught adodb.Stream are making AVs going crazy because most of the old viruses
were using it to inject files on computers. Obviously, the injected code will NOT be executed as it is contained within an image or a video
but AVs will read the content(image cache in discord directory) and will see the syntax and will try to block it and tells you that something
is dangerous in the repertory.

If you came here to check what the hell is that well it is not dangerous and yes i understand that peoples panic when they see that but don't worry
there's no indian scammer trying to rat you with an image.
<img src="https://github.com/TaxMachine/discord-virus-injector/raw/main/virutotal.png">
## How to disable the trigger
 - Go in your windows defender settings
 - Go in Virus and Threat protection
 - Scroll down and go to 'exclusion'
 - Add exclusion(directory)
 - And put this path `C:\Users\YOURNAME\AppData\Roaming\discord`

## Injector Documentation
Put your images/gif/videos in a folder called `toInject`<br>
**BE SURE TO PUT THE DIRECTORY YOU ARE WORKING IN IN EXCLUSION**<br>
start the script with
```cmd
python injector.py
```
and all the images should have the code injected
### Accepted format
```
png
jpg
jpeg
jfif
mov
mp4
webm
webp
```
