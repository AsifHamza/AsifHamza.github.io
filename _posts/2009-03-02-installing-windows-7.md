---
layout: post
title: Installing Windows 7
date: 2009-03-02 18:27:37.000000000 +02:00
social-share: false
tags: [Vista, Windows 7]

---
## Vista’s not that Bad

I must admit that I was taken in by all the negative press surrounding Windows Vista. So when my company decided to upgrade my laptop OS to Vista, I tried everything humanely possible to try and stay on Windows XP. 

But they wouldn’t budge. And so, with great trepidation I started using Vista and found…………… *I actually like it.* It does take getting used to if you, like me, have been using XP for going on 5 years, but I haven’t experienced any of the horror stories I’ve read about. 

There have been times where I’ve run into a problem that had me stumped, like copying my <a href="http://technet.microsoft.com/en-us/sysinternals/0e18b180-9b7a-4c49-8120-c47c5a693683.aspx">Sysinternals</a> applications to the program files directory and not finding them there afterwards (<em><a href="http://www.itwriting.com/blog/141-peeking-into-vistas-virtual-store.html">tip: Learn about Vista’s Virtual Store</a></em>) but on the whole it does feel a lot snappier than XP.

## Installing Windows 7 from a bootable CD
My current OS is Windows XP SP3, so to install windows 7, I had to perform a clean install as the upgrade option only works if you upgrading from Vista. This meant spending a night backing up everything on my machine. Once that was done I could tell the installer to format my hard drive and perform a clean install.

That’s when my problems started. The installer copied the files across but then got stuck on 0% at the expanding files stage. Finally it came back with an obscure error message: Error 0x80070001. 
A quick search on Google for <a href="http://www.google.co.za/search?q=Windows+7+install+error+0x80070001">“Windows 7 install error 0x80070001”</a> did not provide any useful information. 

The closest I found was someone advising to burn the image on 1x speed in the burner as its most likely a DVD burn problem. Another guy suggested removing all connected USB peripherals. None of these solutions worked.
I double checked the SH1 hash of the downloaded ISO to make sure the ISO was valid. It was. Oh crap! This must be Redmond punishment for believable all the negative Vista press.
After sleeping on the problem for a night, I came up with the idea if installing via a 4GB memory stick. 

## Installing Windows 7 from a bootable flash drive
Modern BIOS’s have the ability to boot via a memory stick. Mine doesn’t. But I only found that out *after* I had created a bootable memory stick by following <a href="http://maketecheasier.com/boot-and-install-windows-7-from-usb-flash-drive/2009/01/23">these instructions</a>. 

I created the bootable flash drive from Vista as no additional download was necessary. That’s when I found out I my BIOS did not support USB as a bootable device.
“No problem”, I naively thought. “I’ll just get the latest BIOS firmware for my motherboard”. Luckily for me, the latest firmware did support booting from USB. And they provided flash file for Vista and DOS. And that’s when I realized that with no OS on my machine ( the windows 7 installer had formatted by main partition), there was no way I could run a firmware upgrade. Double crap!

“No problem”, I naively thought again. “I’ll just create DOS bootable CD”. That was easier said than done. All the methods to create a bootable DOS cd just did not seem to work under Vista. And creating a Vista bootable disk was out of the question since I did not have the original Vista cd (this being a company laptop).

That's when I came upon the a truly brilliant idea.

## Installing Windows 7 from a bootable flash drive <em>and</em> a bootable CD
When I tried to install Windows 7 from a bootable CD, I noticed that there was a repair option. You could get to a command prompt via this option. Would it be possible to access the flash drive via the command prompt? Yes <strike>we</strike> you can! So I popped in the flash drive and a short while later …….
<a href="http://asifhamza.com/wp-content/uploads/2009/03/win7peek-after.jpg"><img title="Win7peek_after" style="display:block;float:none;margin-left:auto;margin-right:auto;border-width:0;" height="224" alt="Win7peek_after" src="{{ site.baseurl }}/assets/win7peek-after-thumb.jpg" width="297" border="0" /></a> 

Okay so the above screenshot is not actually taken from my machine (got it from the Microsoft site) but it looks pretty much the same. Except for the weird date. 

I’ve been using Windows 7 for about a month now and its remarkably stable for a beta. The only issues I’ve been experiencing is a missing Canon Pixma Ip5000 driver and a scrambled image whenever the UAC dialogue pops up. The canon driver is a problem on my laptop as well while the scrambled image seems to be a common Nvidia Vista driver problem with certain cards in 7 series range.
