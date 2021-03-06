# ttaudio - TipToi Audio

ttaudio converts a collection of *.mp3 or *.ogg audio files into a single *.gme file to play on the [Ravensburger TipToi](https://www.ravensburger.de/shop/tiptoi/index.html) pen.

**IMPORTANT:**  
ttaudio is neither offered nor supported by Ravensburger. All information shown here was consolidated by independent hobbyists and only for educational purposes. The authors do not take any liability for possible damages.

## Main Window

![Screenshot of MainForm](/doc/screenshot_mainform.png)

## HTML output

![Screenshot of HTML output](/doc/screenshot_html_output.png)

## Workflow
* Attach the TipToi pen to the USB port of your computer
* Start ttaudio
* Drop audio files into the file list
* Click `menu -> Build -> Upload to Pen`
* The conversion of audio files starts
* A web page with optical IDs to play the audio files opens
* Print the web page
  * Use a printer with at least 600 dpi black-and-white resolution. 
  * Disable all "Toner Saving" or "Eco-Mode" settings. 
  * Check the [list of supported printers](https://github.com/entropia/tip-toi-reveng/wiki/Printing)
* Wait until ttaudio has copied the *.gme file to the pen

## More possibilities

ttaudio is based on [tttool](http://tttool.entropia.de/), a universal, command line based tool to create and analyze GME files. 
Check out http://tttool.entropia.de/ if you want to do more than just upload some MP3 files, e.g. print your own interactive books or toys.

## Dependencies

Internally, ttaudio uses following tools:
* [mpg123-1.22.0-x86-64](http://www.mpg123.de/download.shtml) to decode mp3 files
* [oggenc2.exe](http://www.rarewares.org/ogg-oggenc.php) to encode the ogg files for the audio pen
* [oggdec.exe](http://www.rarewares.org/ogg-oggdec.php) to decode input *.ogg files
* [tttool-win32-1.5.1](https://github.com/entropia/tip-toi-reveng) to assemble the *.gme files

