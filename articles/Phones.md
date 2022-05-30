---
name: How to pick a phone without being used by it. 
description: Most of modern phones are having you and you data hostages, essentially making you a slave. How to evade it? Let's find out.
img: rms-on-iot-meme
img-alt: meme text
---

# Operating Systems
At the moment we are really (and I mean **really**) limited in our choice of mobile operating systems. Mostly iOS or Android.

## iOS
Fortunately or not, I have [already made up my mind about Apple products](../on-apple). If you don't value your sanity, freedom, and privacy, their products may be right for you, although there is far less software available for iOS than for Android. If you are a *mobile gamer*, be warned, there are no decent emulators for iOS. Even on jailbroken devices. Sorry, it's too much of a hassle to maintain a full emulator for 0.05% of people (and that percentage is shrinking!). Accessories like gamepads are also expensive or non-existent.

![Quickpwn's logo (iOS jailbreak tool)](https://upload.wikimedia.org/wikipedia/commons/0/07/Quickpwn.png)

## Android
It's Complicated. As a general rule, Android is horrible.
1. Manufacturers [ignore specs](https://dontkillmyapp.com/), lock the bootloader of *your* (in this case, is it really your phone?) phone, blocking root access from you
2. They also steal all your data.
3. The development culture is also very, shall we say, old-school. It seems that most Android developers somehow don't know how free software is developed. Most of them spend their time on the XDA forum in their own thread, giving incorrect answers to repeated questions from confused users. There is no public git repository, bug tracker, or documentation. The only thing there is: a glued bunch of binary files. Some of these things have to do with the fact that drivers for most devices are closed source. Android is also a relatively young platform. Some developers have very little (if any) understanding of how free software development works.
4. Peripheral support is mediocre at best, forcing developers to reinvent the wheel. (I'm not familiar with the underlying mechanics of this and am just judging from my own UX).

Pros:
That being said, I still have to admit: Android is far from the worst mobile OS. Mainly because most of the problems mentioned can be worked around.
1. Android is actually not that bad in terms of running *side-loaded* apps. The way it isolates apps is really decent, and it's pretty hard for malware to escape isolation if your Android is **done right**. The only problem is that it probably isn't.
2. There is a huge amount of software available, which is a good thing. Some of these programs are of poor quality or are malicious, which is bad.
3. Android **can** be done right. However, it still won't be the perfect operating system. You'll still be using huge, bloated, battery draining *super apps*. In a sense, this is a consequence of how Android works.
4. Peripherals are much cheaper and generally better supported.



## PostmarketOS
This is the most interesting option **for me**. PostmarketOS actually is a full-blown ~~gnu~~ Linux based on [Alpine](https://alpinelinux.org/about/).
I'll start with the cons:
1. Slightly worse software availability than Android. It's not easy to get some programs to work. And some really limited amount of software won't work at all (as of 5/29/2022).
2. A very limited number of devices are supported. This is directly related to the closed source drivers, so the team cannot be blamed for this.
3. Officially supported devices are much slower than Android flagship phones.
4. The cameras may not be the best for most phones, although the [Pinephone pro]() looks decent at least.

At the same time, I still consider PostmarketOS the most promising and suitable option for me for the following reasons:
1. Anything you can do with Linux can be done with PostmarketOS.
2. In terms of security, it can be considered more secure than android (although debatable, but I consider it more secure).
3. You can run most Android applications with a few options (e.g. [Waydroid](https://wiki.postmarketos.org/wiki/Waydroid)).
4. Development culture is much better too! Unified gitlab repository, bug tracking system and all that really is a dream compared to XDA.
5. Support for peripheral devices is at point. You can also easily customize, debug and remap keys for your peripherals.

## What about other operating systems/distros?

I don't think they're worth your time. However, don't take my word for it — it's cool if you find something that suits you better. For example, I may be unfair to [GrapheneOS](https://grapheneos.org/faq#supported-devices), but for me it looks shady that they only support Google phones. Still, their arguments seem reasonable, so I can't complain much. 

# So, how to actually pick a device?

## How to pick an Android device

For Android you are looking for at least:
1. The bootloader is unlocked or at least can be unlocked
2. Ability to gain root level privileges as a result.

The only *Android distribution* I can recommend is [LineageOS](https://www.lineageos.org/), for this reason I recommend checking out the [list of officially supported devices](https://wiki.lineageos. org/devices/).
There are many phones that work flawlessly on Android that are not officially supported by LinegeOS (check this before you buy), however you may need to compile it yourself specifically for your phone. Please do not download sketchy images from the XDA forum. It can be malicious and your phone always keeps the most sensitive information.

### Google services

Please, don't install Google services on your phone. For example, instead of play market I'd recommend [F-droid](https://f-droid.org/). Yes, some of software here is outdated, but it's still privacy respecting and it won't be outdated as long as original developer cares enough.
If you absolutely need some of google services, consider using micro-g. I myself wouldn't do that, but it's just in case you absolutely need Google services. 

## How to pick a device running PostmarketOS

Well, with PostmarketOS everything is much easier. The list of supported hardware is really limited so far. These are mainly [Librem](https://puri.sm/products/librem-5/) and [Pinephone](https://www.pine64.org/pinephone/) phones. I would prefer the SIM module to be isolated for security purposes if you ask me. At the moment it's Pinephone for sure. I'm not into mobile gaming so I don't need a powerful processor and all, although I can still play my favorite Street Fighter 3rd strike at full speed. As a bonus, I can connect peripherals like gamepads, arcade sticks and all.

>! Some video here
