---
layout: post
title:  "Data Bending for Fun!"
date:   2021-06-02 21:37:50 -0400
categories: computer-art
---

As everyone knows, computers have a purpose of working with data. You feed data into a computer; new data comes back. This data will serve all kinds of purposes.

But computers can, and have always been, used for creative endeavors, too! Art, movies, music, games (of course!)... computers have been there to do it all!

But today, I want to show off a little something known as databending, or, in layman's terms: screwing around with data and making crazy-ass shit!

![An example of databending, taken from Wikipedia](/assets/databend-example.png)

Databending is basically taking a media file of any sort and manipulating it in ways it was not meant to be manipulated. For example, you could do something like, say, take an image file and open it in a text editor, then go in and start either copying blocks of the data around, or injecting in some random strings of characters, and then saving it back, which often creates a wild, glitchy, beautiful mess. And on that note, I would like to also mention that glitch art and databending do go hand in hand; by doing databending, you're glitching out the data and creating art!

As an example, here's a photo I shot with my old HTC Magic about 11 years ago, unaltered:

![A photo before databending](/assets/light-paint.jpg)

And here's the same photo, after I opened the image in Notepad for Windows and began messing with strings and blocks of data:

![The same photo after databending](/assets/glitched.jpg)

Pretty wild, right?

But opening in a text editor is just one way of doing things. You can also open an image file in an audio editor like [Audacity](https://www.audacityteam.org/), for example, and manipulate it as if it were an audio file. I'll give an example of that now!

Let's take our original, unaltered image; here's a photo I took in New Orleans a few years ago that'll be our tester:

![Surveyor of all this bar](/assets/jester-unbent.jpg)

To prepare, it's best to have the image be in an umcompressed format first; I recommend saving your image as a TIFF file with either GIMP or ImageMagick (if you're on Linux or a Unix; otherwise Photoshop will do the job on Windows or macOS).

Once you have your TIFF file saved, it's time to launch Audacity. In Audacity, go to File > Import > Raw Data...

![Importing raw data in Audacity](/assets/audacity1.png)

...and navigate to where you saved the TIFF image.

![Ahh, there you are!](/assets/audacity2.png)

The settings to use are as follows:

- Encoding: U-Law
- Byte order: Big-endian
- Channels: 1 (Mono)

![The best settings](/assets/audacity3.png)

And now you should see the data as an audio track!

![Time to have some fun!](/assets/audacity4.png)

Now at this point, you're probably asking yourself, "Well, what to do now?" The answer to that is ***whatever strikes your fancy!*** Audacity is chock full of effects to apply to your "audio", but to start off, let's try messing with the header first, and maybe throwing in a couple of echo effects. Select the first 5 seconds of the audio track, then select "Echo" from the Effect menu. You can leave the settings as they are, and just click "OK". This will apply your echo effect to the header!

![Echo effect applied!](/assets/audacity5.png)

Now go through the audio stream and try playing with the echo effect at random places; what you're effectively doing is duplicating random chunks of data here. Once you feel you've done enough, it's time to export the data back out! From the File menu, select Export > Export Audio...

![Time to export our data](/assets/audacity6.png)

And in the Format Options section, select "RAW (Header-less)" for the header option, and "U-Law" for the encoding option. Be sure to change the file extension before saving (I recommend using .bmp as the extension to save the data as a bitmap image), and go ahead and hit "Save". You'll have the exported data saved, which you can then take a look at to see the results of your handiwork!

![Whoa, that's wild!](/assets/jester3.png)

Fun stuff, ain't it?

Now for another example of databending: taking a pure audio stream and exporting it as an image. You can also do this in Audacity by opening an audio file of any sort, and exporting it similarly to the example above. Here's an example I created from an extracted bit of audio from, off all things, a K-Mart announcement cassette that I found on the [Internet Archive](https://archive.org/details/attentionkmartshoppers)!

![It's not announcing a Blue Light Special!](/assets/1962.jpg)

Now, let's see what an image sounds like! Here's our example image:

![Strange Lights](/assets/strange-lights.jpg)

I loaded this image into Audacity, exported out the audio as a WAV, and then combined the two together so you could ***hear*** the image as well as see it. The results are... well, here ya go:

[![Strange Lights](https://img.youtube.com/vi/vd7Oo8Ly9yo/0.jpg)](https://youtu.be/vd7Oo8Ly9yo "Strange Lights")

Pretty freaky sounding stuff!

All in all, databending and glitch art are fun hacks to data that some don't really think of outside of the realm of "create" and "display". We are "creating", but perhaps it's creating by breaking? We create weird beauty from something broken? Are we breaking our visions of what reality is? Are we circumventing the notions of reality? Who knows! But I do have to say that creating glitch art and doing databending is a fun process, and there are many, many more ways of trashing data in the name of art out there. If you'd like to get started making your own glitch art, a quick search in your favorite search engine will turn up some good results for generators, where you can load an image up and screw with it to your heart's content. But I do implore you all: get out there and have some fun. Make crazy shit. Go wild. Enjoy yourselves. There's no right or wrong way to do it!

Happy hacking, everyone! :)