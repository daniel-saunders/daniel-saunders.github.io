---
layout: default
title: Chromebook
---

# An all-round travel laptop for £60 pounds - Chromebook + GalliumOS
### July 2017

## Introduction
How cheap can a laptop be whilst still offering all the required functionality for a developer? I asked this question just after finishing my PhD, when I realised I wanted a cheap laptop for home and travel (to avoid taking my expensive work laptop that's perfectly setup for my research). The requirements I had in mind:

* Suitable for web browsing
* Ability to login to external machines using `ssh` (inc. showing external graphics)
* Manage emails
* Enough resources for light development (trying out ideas on the go)
* Lightweight gaming

It turns out this can be achieved for very little indeed! 
Since we'll be using an open source OS (to avoid buying a windows licence, and to choose something more lightweight), this is the perfect choice for someone wanting a cheap introduction to running Linux.

## Hardware
So what can £50-£100 provide in terms of hardware? A quick look on eBay reveals the following broad categories:

* Old laptops for spares/repairs. These laptops typically require a bit of work and more money to get running, and so are beyond the budget of this article - for an example of this category, see [here](revived_ultrabook.md)
* Netbooks: all-round mini laptops that run windows on light hardware
* Chromebooks: googles version of a lightweight laptop, designed purely for web browsing, also on light hardware

Chromebooks are an interesting option that I hadn't thought about previously. They run ChromeOS by default, which is itself based on Linux, so Linux compatibility isn't a problem. In terms of cost, I noticed that frequently they sold for *cheaper* than the netbooks (for similar hardware); eBay seems to have plenty of unwanted chromebooks, presumably due to lack of awareness of their intended use and capabilities. I payed £60 for a HP Chromebook 11 G3, which has the following specs:

* 11.6 inch screen
* Intel Celeron N2840. This will be a bottlekneck for some applications, but it turns out not to be that bad 
* 4 GB of RAM - I wouldn't go for less
* 16 GB SSD hard-drive - small, but it also has an SD card slot that can be used to add extra capacity

Note: you'll want an Intel based CPU if you want to run some of the Linux distributions recommend below. 
An upside of such low specs is less power usage, so we can expect impressive battery use (see later). 

## Software & OS
With these low specs, the choice of OS is vital. A common misconception is that older computers pass some kind of expiry date, after which they *just won't work*. Whilst this is certainly the experience of many windows users, the cause of this is not routed in hardware - the hardware doesn't change in time - but software does. Windows is a comparatively heavy operating system, and gets heavier as time goes on with updates. This is the big problem for the windows-based notebooks, which seem to give up very quickly. The solution for low resource hardware is a lightweight OS, and there are many suitable Linux distributions. Note: this does not mean the laptop functionality is hindered - of all the requirements listed above, only web-browsing is getting more intensive as time goes on (the resources needed to run everything else havn't really increased much in the last decade).

ChromeOS itself is getting better day-by-day, and for many people may already be a better alternative to Windows or MacOS. It has a very clean and intuitive interface, much like a tablet, and has been designed for simplicity and reliability. This comes at the expense of hiding many features from the user, which as a developer is why i didn't give it much more time. On the other hand, I'm seriously considering getting my mum to switch.

There are a few different [ways to run Linux on a chromebook](https://arstechnica.com/gadgets/2017/06/how-to-install-linux-on-a-chromebook/). For newer chromebooks, there are even more options offered by [google themselves](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwifoO3m3NHfAhVrSxUIHT8dALQQFjAAegQICBAB&url=https%3A%2F%2Fwww.zdnet.com%2Farticle%2Fhow-to-add-linux-to-your-chromebook%2F&usg=AOvVaw30EGvv4f1Uz_AbkPIKjY3O). After trying out a few options, I opted for a full install of [GalliumOS](https://galliumos.org/). GalliumOS is based on Xubuntu, which happens to be my default goto Linux distribution for most purposes, and was also the snappiest distribution I tried out. This is essentially a stripped down version of Ubuntu, using XFCE as a desktop environment (a favourite amongst developers), with the chromebook drivers included. The documentation is also excellent, with compatibility notes for most chromebook models. 

The usual disclaimer applies when running Linux: there will be some *small* pain in getting things to work initially. 


## Experience
My mind is blown...

I could almost spend all my time using this laptop and be just as content and productive. It can do everything i'd hoped for and more. Compared to my work ultrabook, there are only a handful of cases where I notice a difference day-to-day:

* The weak CPU can make web browsing a *little* sluggish, particularly for ad heavy websites. 
* The small hard-drive means constantly being aware of where large files live. An SD card helped this, although this is a bit cumbersome.

Everything else is awesome. The battery life is very impressive given the low specs - i frequently get 6 hours of holiday usage (easily twice my work laptop, even doing the same tasks). GalliumOS feels just as familiar as other Ubuntu based distributions, and i haven't run into any software compatibility issues - I've even been able to perform some lighter machine learning analysis! I've used this laptop as a stand-in to my work laptop on many occasions, including writing and presenting several conference talks. If I were often running more computationally heavy tasks, I may've run into more problems; but on the other hand, those tasks are typically ran on external servers anyway. 


## Conclusion
All the requirements I set out were fulfilled and beyond for just £60. Chromebooks offer amazing productivity per pound of hardware, and given a large market on eBay, they can be picked up for a bargain on eBay. GalliumOS is very impressive in terms of documentation and compatibility, offering a familiar feel for developers. This is an excellent option for those wanting a cheap way to try out Linux as an OS, or just about anyone who'd like a cheaper laptop that covers almost all day-to-day tasks.

Before this experiment, I'd planned on selling my Chromebook on after these trials, but now i think i'll construct a plinth for it. Ironically, its value to me now far exceeds £60.
