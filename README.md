# openwith-waterfox-linux
Fix for the firefox extension OpenWith to work with Waterfox 6.x.x

I should note something important -  a fair warning: I'm not a developer, so these modifications will work until Waterfox make some fundamental changes on how extensions work with the browser. If or when that happens and the xpi stops working with the browser, my modifications will also stop working. I can read and edit code to a certain degree, if or when necessary, but I can't write code from scratch.

As you probably already know, "Open With" (OW, for short) was mainly used with Firefox and later received a fix to work with Waterfox Current. However, at some point of the waterfox's development, that name disappeared and it's now named just "Waterfox". For whatever reason, OW refused to work with Waterfox 6.x.x versions and displayed a red badge with exclamation mark and message like "Open With could not connect to the outside world".
Despite the fact that OW.xpi file hasn't been updated for several years, I still managed to make its latest version 7.2.6  work with Waterfox 6.5.10. Note that I HAVEN'T edited the xpi file, so the extension will still appear as OW by darktrojan.
Anyway, my fix goes outside the xpi file.

ALL YOU NEED TO DO is simply download the '.py' file from my repository, place it wherever you want, run

```
./open_with_linux.py install
```
and then click the button "Test installation". As I've discovered, on some distros you may have to run this as sudo, especially if you've stored the file on the root partition. If  you see green, everything's OK. If it's red, check if you have python3 installed.

There's NO NEED to download the xpi from here, I've added it, so that you don't have to jump to the mozilla's extensions page to search for it.
The main thing you need from here is the '.py' file which was permanently fixed to work with Waterfox, unless they change the browser name again.

I suppose I could try to make it work with Waterfox Classic but I don't have this browser and no way of knowing whether OW will work AT ALL with the Classic version.

Linux and Windows version were fixed and confirmed to work. Working on the Mac version. This thing is mostly an endless JSON code on a single line which makes it diffucult to find the part I need to edit.
