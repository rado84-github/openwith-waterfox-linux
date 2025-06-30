# openwith-waterfox-linux
Fix for the firefox extension OpenWith to work with Waterfox 6.x.x

As you probably already know, "Open With" (OW, for short) was mainly used with Firefox and later received a fix to work with Waterfox Current. However, at some point of the waterfox's development, that name disappeared and it's now named just "Waterfox". For whatever reason, OW refused to work with Waterfox 6.x.x versions and displayed a red badge with exclamation mark and message like "Open With could not connect to the outside world".
Despite the fact that OW.xpi file hasn't been updated for several years, I still managed to make its latest version 7.2.6  work with Waterfox 6.5.10. Note that I HAVEN'T edited the xpi file, so the extension will still appear as OW by darktrojan.
Anyway, my fix goes outside the xpi file.

ALL YOU NEED TO DO is simply download the '.py' file from my repository, place it wherever you want, run

```
./open_with_linux.py install
```
and the click the button "Test installation".
If  you see green, everything's OK. If it's red, check if you have python3 installed.

There's NO NEED to download the xpi from here, I've added it, so that you don't have to jump to the mozilla's extensions page to search for it.
The main thing you need from here is the '.py' file which was permanently fixed to work with Waterfox, unless they change the browser name again.

I suppose I could try to make it work with Waterfox Classic but I don't have this browser and no way of knowing whether OW will work AT ALL with the Classic version.

For Windows: if you want fix for Windows, I'll need the python file for Windows because I don't have it. You could open a request as an issue and upload the file for Windows. Then I'll fix it there too and I'll add it to this repository.
