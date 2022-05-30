---
name: How to pick a phone without being used by it. 
description: Most of modern phones are having you and you data hostages, essentially making you a slave. How to evade it? Let's find out.
img: rms-on-iot-meme
img-alt: meme text
---

# Operating systems
At the moment we are really (and I mean **really**) limited in choice for mobile operating systems. Mainly, it's either iOS or Android.
##iOS
Fortunately or not, I [already made my mind on Apple's products](../on-apple). If you don't value your sanity, freedom and privacy, it might still work for you, although there's much less software available for you on iOS then on an Android. If you're a *mobile gamer* — beware, there's no decent emulators for iOS, and you're really missing decent games because of that. Even with jailbreaked devices. Sorry, it's too much of a hassle to support full-blown emulator for 0.05% people (and this precent is declining!). Accessories, such as gamepads are also pricey or non-existent. 

##Android
That's a tricky one. Typically, it's horrible. 1.Manufacturers are [ignoring specs](https://dontkillmyapp.com/), locking bootloader of *your* (is it actually your phone in this case?) phone, locking root access from you
2.They are also grabbing all your data. 3.Development culture is also really, let's say, old-school. It feels like most android developers are somehow unaware of how open source projects are done. Most of em are wasting their time on XDA forum on their own thread, giving wrong answers on repeating questions by confused users. There's no public g it repository nor bug tracker or documentation. The only thing there's: binary files sticked together with a glue. Some of this things are a consequences of the fact, that drivers for most things are closed source. Android is also a relatively young platform. Some developers have really brief (If some) idea about open-source.
4.Support of peripheral devices is mediocre at best. 

For a good things: 
With this being said, I still have to admit: Android is far from being the worst mobile OS. Mainly, because most of mentioned problems can be evaded. 
1.Android is really not that bad in terms of running *side-loaded* apps. The way it isolates apps is really decent and it's kinda hard for malicious software to escape it, if your Android **done right**. The only problem — most likely it's not. 
2.There's a huge pile of software available, which is a good thing. Some of it is low quality or malicious, which is a bad thing.
3.Android **can** be done right. Still, it won't make a perfect operating system. You're still using huge, bloated, battery-draining *super-apps*. Some of it is, in fact, a consequence of the way Android works.
4.Peripherial devices are much cheaper and better supported overall

##PostmarketOS
That's most interesting option **for me** PostmarketOS is, infact, a full-blown Linux phone operating system, based on [Alpine](https://alpinelinux.org/about/).
I'll start with bad things about it:
1.A bit worse software availability than an Android. It's not that easy to make some software work. And some really limited amount of software won't work at all (for now as 29.05.2022).
2.Very limited amount of devices is supported. It have something to do with drivers being closed source though, so can't blame the team for it.
3.Oficially supported devices are much slower, than flagship android phones are.
4.Cameras can be far from being good for most phones, although "Pinephone pro" seems to be at least decent.

With this being said, I still consider PostmarketOS most perspective and suitable option for me for this reasons: 
1.Anything you can do with Linux, can be done with PostmarketOS. 
2.In terms of security, it can be considered more secure, than an android (although debatable, but I consider it more secure). 3.You can run most Android apps via handful of options (e.g. [Waydroid](https://wiki.postmarketos.org/wiki/Waydroid)).
4.Development culture is also much better too! Unified gitlab repository, bugtracker and all of that, which really is a dream compared to the XDA thing.
5.Peripherials support is on point. You can also easily tweak, debug and remap keys for your peripheral devices (something Android can't reach till this very day, making everyone reinvent the wheel) 

##So what about other operating systems/distros?

I don't think they're worth your time. Still, don't take my word for it — it's cool if you'll find something that suits you better. For example, I might be not fair to [GrapheneOS](https://grapheneos.org/faq#supported-devices), but for me it looks shady that they only support Google phones. Still, their arguments seem reasonable so I can't complain much. 

#So, how to actually pick a device?

##How to pick an Android device

For an Android, you're looking for, at least:
1.Bootloader unlocked or at least unlockable
2.An ability to get a root-level privelleges as a result.

The only "Android distro* I can recommend is the [LineageOS](https://www.lineageos.org/), for this reason, I recommend to get familiar with [list of officially supported devices](https://wiki.lineageos.org/devices/). 
There's plenty of phones that work flawlessly on Android while not being officially supported by LinegeOS (check it out before buying), though, you might need to compile it yourself specifically for your phone. Please, don't download sketchy images off of XDA forum. It might be malicious, and your phone always store your most sensitive information.
###Google services
Please, don't install Google services on your phone. For example, instead of play market I'd recommend [F-droid](https://f-droid.org/). Yes, some of software here is outdated, but it's still privacy respecting and it won't be outdated as long as original developer cares enough.
If you absolutely need some of google services, consider using micro-g. I myself wouldn't do that, but it's just in case you absolutely need Micro-G. 

##How to pick a device running PostmarketOS

Well, it's much simpler with PostmarketOS. The list of supported hardware is really limited for now. Mostly it's Librem and Pinephone phones. I'd look for one with isolated SIM module for additional security, if you ask me. For now it's Pinephone for sure. I'm not much of a mobile gamer tho so I don't really need powerful CPU and all of that, although I will still be able to play my beloved Street fighter 3rd strike at fullspeed. As a bonus, I get to connect peripheral devices, such as gamepads, arcade stick and all of that.

>! Some video here