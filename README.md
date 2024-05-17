# FlipperMusicRTTTL

Selection of RTTTL `.txt` files that will work with the FIipperZero Music Player. 

## Instructions

### First time instructions

1. Plug in your Flipper Zero
2. Open up qFlipper
3. In qFlipper, click the third tab that looks like a file.
4. Create a file on your `SD Card/apps_data` folder called `music_player`, if it doesn't exit.

### After the first time

1. Drag one of the folders in this project into `SD Card/apps_data/music_player/`
    - `ArcadeTones`
    - `RTTTL_generics`
    - `Theme_Songs`
    - `Unsorted 10k Song Archive`
2. Overwrite any future files. The files should be `.fmf` or `.txt`.

## Notes left by @neverfa11ing 

> Put any .fmf or .txt files here so you can see all the songs.
> Thank you *@drshade.* for the info.
> 
> Make sure you are downloading the .txt file and not a .html for them to work.
> 
> Feel free to add or make any changes.
> 
> Adding a new folder called "ArcadeTones", it will contain newer additions.
> 
> When using RingtoneComposer make sure you are exporting as an RTTTL and not saving as a txt file.
> 
> SendTone is usuful for minor edits and is very similar to nokring.
> 
> Nokring is best for composing from scratch, also good for edits.
> 
> ![RTTTL-ringtone-diagram](https://user-images.githubusercontent.com/6899421/171048290-1e95c9ba-5c26-4e6b-a969-ecd6003c6423.gif)
> 
> An online RTTTL player is available here: https://adamonsoon.github.io/rtttl-play/

## OK, back to me

The Flipper Zero can either be this "big scary hacker tool" or it can be fun and useful.  Unfortunately, due to *un certain petit québécois*, Canadians currently can't enjoy the fun parts because it is currently 1995 in Ottawa. And that guy is like the Secret Service agent from a certain bad 90s movie.

Fortunately, I'm in America "Home of the Whopper" as Stephen Colbert would say.

But this "big scarry hacker tool" is being put to good use. And thanks to @neverfa11ing and "@drshade", there is a library of old ringtones that need to be organized...and could also be used to help me with another program I am working on which will turn the Flipper Zero into a guitar chords as well as make RTTTL useful again.

But...if you are a budding guitar person like me, you know that the first note on a guitar on the lowest string in standard E tuning is **E2** ("low E") is seven semitones up from **A1** (55Hz) and five semitones down from **A2** (110Hz), but the guitar's highest string in standard E tuning is **E4** ("high E"), which is seven semitones up from **A3** (220Hz) and five semitones down from ** Standard A4** (440Hz), the lowest note that RTTTL can support. I'm using the [Piano Key Frequencies](https://en.wikipedia.org/wiki/Piano_key_frequencies) defined on the Wikipedia page. There's actually a formula for calculating frequency.

The [RTTTL Format specification](http://merwin.bespin.org/t4a/specs/nokia_rtttl.txt) states that the range on the Nokia 61xx was between **A4** and **B7**.  So what if what you wanted to play on the guitar was shifted up three octaves? This would make **E5** "Low E" and **E7** "High E". And since we need to consider that the hightest note is **B7**, to if we tuned our guitar up two octaves, it would be at the 7th fret, two notes highter than **A7** (3520Hz).

I suspect that the Flipper Zero uses the same range as the Nokia 61xx, so any music that we create will need to be shifted up **THREE** octaves.

However, there's also another hack.  Many rock musicians tune their guitars using **D tuning**, so we can shift our available notes down two notes, making **D5** the lowest. Again, the range starts at **A4**, but **C5** is *Middle/Tenor C*.

The Wikipedia page for [Ring Tone Text Transfer Language](https://simple.wikipedia.org/wiki/Ring_Tone_Text_Transfer_Language) is pretty thorough, but I would still like to add some documentation to this repo.

## TODO List

- [ ] Organize the "10K" ringtones. I might toss out most of them. Text files are easy to compare using Linux. Eventually, we'll use the most well defined ringtones and if there's a different rington for the low tones (A4 to B5) and the high tones (A6 to B7), we'll try to preserve that. There could be some tones that use the mid tones (A5 to B6).
- [ ] Find more ringtones!
- [ ] Create more ringtone! (Wish list item)
- [ ] Use some the the ringtones to build the guitar chord app that I'm interested in making. (It might be a couple of apps. Depending on how I can digitize this old paper computer that will defintely help.

