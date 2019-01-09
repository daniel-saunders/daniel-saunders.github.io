---
layout: default
---

# 30th Oct 2017 - Motivation & first thoughts on components

The time has come to build my first PC by myself. More than anything, this will be a learning experience, to understand where bottlenecks arise from cheaper hardware, and where its ok to go cheap. This machine will ultimately become my home go-to machine, sometimes used as a programming station, and for tinkering with software ideas and home hardware projects. I'm not targeting serious gaming, nor generally intense computing - more-so I'm aiming for something that is ideal for home browsing and programming, with the option of doing some fun stuff with a not-so-expensive GPU. As usual, intense stuff belongs on servers. 

After googling through many articles, I found www.logicalincrements.com to be an extremely useful starting point, giving many pre-planned build recommendations, giving a good indication of what to expect for your money. Although there are many many possible combinations, it quickly became clear that there wasn't much difference between different components of the same price point - mostly, you get what you pay for. So in the following, if given a choice, I usually went for the component I found on promotion. 

For the PC itself (including extremities like screens etc.), I originally wanted to keep the cost low, but going too cheap can have serious impacts on future proofing and potential future upgrades. I'd like to keep the total below £500. 

## Linux Distributions
I've been using Linux for a long time and perfectly content using it as a home OS. Part of the fun using this machine will be trying out various different distributions, so light weight isn't guaranteed (but is likely as I like a snappy response). 

> **Jan 2019 update**: I originally installed debian, with the default desktop XFCE, which ran superbly for the first year. My only problem came when installing drivers for the NVIDIA graphics card. That was quite painful, and after seeing similar problems for performing machine learning on non-ubuntu based distributions, I decided to switch to Xubuntu, and now choose this by default. Similarly, I've had a great (and very similar) experience; but best of all, the graphics card worked right away, even with ML libraries. 

## Components
These choices are the result of forming the logicalincrements *entry*-*modest* option as of 2018. Where possible, to save some cash, I'm happy to buy second hand. Some quick searches suggests that CEX is just as competitive as ebay, whilst giving a one year warrenty. The CEX website is also surprisingly complete when it comes to component listings. For this machines first iteration, this first set of components will include:

* **Motherboard**: [ASROCK B250 Pro](https://www.amazon.co.uk/ASROCK-B250M-PRO4-Elegant-Motherboard/dp/B01N0LMLMM/ref=sr_1_1?s=computers&ie=UTF8&qid=1511738958&sr=1-1&keywords=asrock+b250+pro4), £48 - I got this almost half price. When choosing a mother board, the main thing to consider is the available ports (external and on the board itself). In-particular, check the position of the graphics card slots and whether you need a NVMe port.
* **RAM**: 4 GB single stick DDR4 2400 MHz, £30 - second hand from CEX (with 2 year free warranty). 

> **Oct 2018 update**: I've since upgraded to 8 GB of RAM for an additional £40 for more flexible ML. When getting the second stick, ensure the model is *exactly* the same as the first. As well as a RAM boost, you'll enable dual channel mode (presuming your CPU and board allow for that), resulting in a worth-while performance increase. That said, I'm still convinced 4 GB of RAM is fine for everyday needs (and even many ML tasks).

* **Harddrive**: [Samsung EVO NVMe 256 GB](https://www.amazon.co.uk/Samsung-M-2-2280-500GB-Express-Solid/dp/B01M211K53/?tag=logicaincre05-21&th=1), £116. This is the only component I question looking back. I went for NVMe for increased I/O speed. Since then, other SSD costs using SATA3 have often been on offer, and unfortunately, NVMe drive performance has been hit by the Intel Meltdown & Spectre vulnerabilities. Oh well, win some, loose some.

* **CPU**: [G4560  (with cooler)](http://cpu.userbenchmark.com/Compare/Intel-Pentium-G4560-vs-Intel-Core-i3-6100/3892vs3511), £58 (2nd hand, ebay). I love this CPU. Its basically an i3 6th Gen, at around half its cost. Its the first Pentium CPU to allow hyperthreading. The clockspeed is about 10% lower than the current i3, but its not noticeable for every-day tasks. CPU choice can affect GPU performance (i.e this budget card can bottlekneck an expensive GPU. The inverse is also true. It turns out this combination is quite common and pair well). I went for Intel as I was surrounded by people who have relevant experience at work. Nowadays, I'd have to think twice about AMD, as they offer excellent price per cost. 

* **Tower case**: [CiT Dark Soul](https://www.amazon.co.uk/dp/B01MSE30WA/ref=twister_B074G83KSZ?_encoding=UTF8&psc=1), £30. Cheap and cheerful. Check the size of the case matches at least the size of your motherboard with GPU.

* PSU: [EVGA 500 B1](https://www.amazon.co.uk/EVGA-Bronze-Power-Supply-Unit/dp/B01F67KZEC/?tag=logicaincre05-21), £55. Ensure it will have enough power for what you'll need. 

>* **Update Jan 2018: GPU:** [NVIDIA 1050 Ti](https://www.amazon.co.uk/Gigabyte-Nvidia-GV-N105TD5-4GD-GDDR5-PCI/dp/B01M6ZANMP/ref=sr_1_7?s=computers&ie=UTF8&qid=1547071266&sr=1-7&keywords=1050+ti), (4GB vRAM), £150. This is often considered an entry level GPU for doing ML, with gaming performance similar to that of a PS4. vRAM is important here, as this might prevent some ML tasks (ML libraries that run on GPUs have a lot of overhead - tensorflow requires 2 GB just to get started for a task).

> I actually put off buying a GPU for a while, and just used the CPUs internal GPU for day-to-day tasks. This worked well, even for a bunch of games, and can be a great way to save money if you're not bothered about simpler graphics. 

*Total spend: £527 (£337 without upgrades, £270 with a cheaper SSD still)*

## Summary (updated Jan 2019)
This cost is actually a bit more expensive than what logicalincrements would suggest (as of Jan 2019) given the CPU and GPU combination. This change is due to a drop in RAM costs over the last year, and by using a cheaper non-NVMe SSD (as looking back, I would have done. On the other hand, it is very fast). 

This machine does fullfill its aims very well. Its an excellent entry level machine for doing useful ML tasks on a GPU, and is great for day-to-day tasks. I also learnt a huge amount in choosing components and the assembly, which is very satisfying. Highly recommended for computing enthusiasts!

### Notes on extremities
For extremities, I had a decent mouse and keyboard lying around. I'm a huge fan of a dual monitor setup, and found an incredible deal on eBay for a pair of 22-inch DELL screens for £25 (discounted for London collect only ;)) . They're old and very heavy, but who cares, they work very well (they even come with a decent speaker). Combined with a dual monitor stand, they're just what I want. 