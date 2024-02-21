# National Parks Road Trip Summer 2023 - Video Sorting and Organization
This is the process documentation of sorting and organizing all the video files I have of the drives we took during our road trip. 

I don't know why I didn't buy a GoPro, a dashcam, or a different device to capture the drives we had, but I didn't. I instead purchased a new phone, which, now that I think about it, is very strange, and my stubbornness led me to not create a new iCloud account or anything which in retrospect would have made a lot of sense considering how much space I ended up requiring -- either way, I ultimately ran into the issue of needing more space. Our drives were anywhere between under five minutes if it was a quick to and fro, up to over 10 hours long, depending on the leg of our trip, which meant that videos I took ended up being sometimes over 30 GB each, which eats a ton of space.

Anyway all of that aside, I was able to record these videos and move them onto a hard drive--for the most part. Any time I was able to immediately airdrop the video onto my laptop to move it onto my hard drive (big yikes) I could delete it and not worry about it taking up space. However, I forgot to turn off the auto-upload to iCloud functionality, which meant that, after the road trip, my iCloud took a field trip and decided to move all of the videos I had stored on my local device to the cloud, which took up all of the space I had.

This would not have been an issue for *checks watch* the past *double takes* five months, if only videos downloaded from iCloud would have the proper "Date Created" tag for the actual date that it was created. I gave up on this project for a while until recently, when I decided it was time to actually demonstrate that I haven't done nothing during my unemployment period, and wanted to maybe use these files to model the time we spent and what we spent it on and create visualizations from that. Anyway, that meant that I still needed to get all the video files and organize them properly. Luckily, this time when I realized that all the videos that already existed on iCloud could simply be... downloaded (lol) all I needed to figure out was how to change the Date Created metadata to reflect the actual date created since, well, all of these files already include the location so I don't have to worry about that part.

All of that aside, what I'm trying to say is that I found a tool called ExifTool (thanks Phil Harvey) and essentially all I have to do now is downlaod all of my videos (from iCloud > More Download Options > Unmodified Originals) to one directory and then use this singular line on Terminal:

```
exiftool '-FileModifyDate<CreationDate' DIR
```

Anyway I'm going to keep adding to this as I go along for documentation purposes. Yay


