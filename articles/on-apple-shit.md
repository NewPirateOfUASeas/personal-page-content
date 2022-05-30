---
name: Please don't buy Apple's products, or how to backup your phone if you have no enough disk space on your primary disk.
description: How to backup your iphone/ipad/ipod if you have no enough disk space on main drive
img: meme-shitting-on-apple
img_alt: text of meme
long: true
---

# Please don't buy Apple's products!

I just wasted 12 hours because apple don't want to make things the way sane people are used to. 

Here's the task: I need to create backup of someone else's iphone on my PC. Tech specs:
SSD 111GB (C:\\)
HDD 931GB (D:\\)
IPhone 12 256GB

I installed ITunes (let's assume that's ok that I can't access file system directly for whatever reason) and Windows. After that, I have around 80GB disk space. Now let's launch ITunes only to find out — there's no way for us to create reserve copy on second drive! You can only save it on main drive!

> It just works

For obvious reasons, copy fails. There's not enough space for backup.
Okay then, guess I'll have to find out where exactly backups are stored, and create hardlink from this directory to D:\\

1.Launch cmd as a root.
2.Execute the following command:

```bat 
cd %Appdata%/Roaming/"Apple Computer"/MobileSync
```

Here's folder named "Backup". None of saved backups was useful for me since none of em were complete, so I just removed it. Keep in mind — it may differ for you so make sure to move your existing backups somewhere else  before going for the next step. 
3.Now, to save backup somewhere else (e.g. D:\Backup\) run the following command:

```bat
mklink /J Backup D:\Backup
``` 

And try to create backup with ITunes once again.
If you're lucky — it will work, congrats! I wasn't that lucky though. I only had **350gb** of disk space on my D:\. Yes, that wasn't enough, although phone only has **256GB**! It failed when backup growed to 358gb since it's obviously ran out of space. How should I know it? How technically illiterate people should be able to use apple devices (keep in mind — they're the target audience)? Why it takes so much skill to use something that, supposedly, *just works*?
Oh and don't tell me I should've used a Mac for this purpose. First: ITunes used for it for last 20 years, apple could make it work better in all of this years. It means, Windows is supported, and no excuses can be done in this regard (for the same reason I didn't use Linux which I run on daily basis. Keep in mind: i never complained about lack of Linux support, although some people would find it a fair criticism) Second: buying Mac you get absolutely dog shit GPU for the price you're paying (although CPU is kinda decent for power efficiency it gives not gonna lie) and to get a model with enough storage (keep in mind, you still should have at least 360GB of disk space alongside with MacOS) you'll need to sell kidney. And third: you're still not getting control over your phone. Not even photos, it's still obfuscated and tied to "photo" app. 

Apple intentionally made it more difficult for you. The fact that backup takes more space than whole memory of initial device is, also, a consequence of apple making it more difficult for you to recover your own data (no, I didn't use backup encryption) 

I'm done jumping through Apple's hoops and they can go screw themselves. Please, don't ask me to help you with your things if it's related to products of this horrible company. Go live in a doomed world you created yourself.