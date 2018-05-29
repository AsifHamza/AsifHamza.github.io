---
layout: post
title: A New look and a New host
date: 2009-04-01 21:28:00.000000000 +02:00
tags: [CSS, Web Design, Web Hosting, XHTML]
social-share: false

---
Last week I decided to make two radical changes to my blog.

1. Create a new a new theme and in the process learn something about CSS and web design.
2. Move my blog from the free <a href="http://www.wordpress.com" target="_blank">wordpress.com</a> hosting site and onto a paid host and in the process learn something about website hosting.

The result is the site you viewing now. Not too shabby for a first attempt. If I don’t say so myself.


## Web Design with CSS and XHTML
I was getting a bit tired of the my current  theme at the time and thought the time was ripe for a bit of a change. But none of the free wordpress themes I found appealed to me. 
I wanted a theme that was easy on the eyes, had fluid columns and was widget ready. After trawling through hundreds of themes, I decided to try my hand at creating one myself. And the more I thought about it, the more excited I became. 
The prevailing wisdom on the web though, is that website design is not for amateurs. You need to consider SEO, readability, colours, and in some countries their are laws on accessibility as well. But nothing ventured, nothing gained.

First, I needed a good book.
I’ve always loved the <a href="http://headfirstlabs.com/" target="_blank">Head First series of books</a> with their fun and witty format. I tend to stick with books that tell story and have lots of colourful pictures. Luckily for me, they have a book on web design.
<div class="wlWriterEditableSmartContent" style="padding-bottom: 0px; margin: 0px; padding-left: 0px; padding-right: 0px; display: inline; float: none; padding-top: 0px">
<table border="0" cellspacing="0" cellpadding="2" width="400">
<tbody>
<tr>
<td width="400" valign="top"><a title="Head First Web Design (A Brain Friendly Guide)" href="http://www.amazon.com/exec/obidos/ASIN/0596520301/assbl05-20"><img style="float:left" src="{{ site.baseurl }}/assets/0596520301.01.MZZZZZZZ.jpg" border="0" alt="" align="left" />Head First Web Design (A Brain Friendly Guide)</a>
<strong>ISBN</strong>: 0596520301<br />
<strong>ISBN-13</strong>: 9780596520304</td>
</tr>
</tbody>
</table>
</div>

Of course, even with a book that’s entertaining to read, I still get a little impatient try things out. So after  reading a first few chapters, I started sketching out a few designs. I settled on a three column design with a header across the page and a menu below that.
Once I had and idea of what I wanted, it was time to put the design into practice. That's where the Head First book falls short. It discusses web **design** but it does teach you website **creation**. Head First has a <a href="http://www.amazon.com/exec/obidos/ASIN/059610197X/assbl05-20" target="_blank">different book</a> on that.

Luckily, a friend loaned me a book on CSS.
<div class="wlWriterEditableSmartContent" style="padding-bottom: 0px; margin: 0px; padding-left: 0px; padding-right: 0px; display: inline; float: none; padding-top: 0px">
<table border="0" cellspacing="0" cellpadding="2" width="400">
<tbody>
<tr>
<td width="400" valign="top"><a title="Stylin' with CSS: A Designer's Guide (2nd Edition) (Voices That Matter)" href="http://www.amazon.com/exec/obidos/ASIN/0321525566/assbl05-20"><img style="float:left" src="{{ site.baseurl }}/assets/0321525566.01.MZZZZZZZ.jpg" border="0" alt="" align="left" />Stylin' with CSS: A Designer's Guide (2nd Edition) (Voices That Matter)</a>
<strong>ISBN</strong>: 0321525566<br />
<strong>ISBN-13</strong>: 9780321525567</td>
</tr>
</tbody>
</table>
</div>

As with the previous book, I went through the first few chapters and learnt the basics of CSS. The syntax was easier and intuitive. But when it came to advanced layout techniques, it was a nightmare. Browser incompatibilities, box model, quirks mode -  I could not get the hang of it fast enough. But <a href="http://matthewjamestaylor.com/" target="_blank">Mathew James Taylor</a> does have the hang of it. He has <a href="http://matthewjamestaylor.com/blog/equal-height-columns-cross-browser-css-no-hacks" target="_blank">tutorials</a> on how to create quirks mode free layouts in CSS. I tried to following one of them but there’s some serious dark magic in there. So I ended up using his <a href="http://matthewjamestaylor.com/blog/ultimate-3-column-holy-grail-pixels.htm" target="_blank">3 column liquid layout</a> instead.
Once the CSS was in place, it was just a matter of playing around with colours and tweaking things here and there, referring to the two books above where necessary, and <a href="http://max.limpag.com/2006/09/01/how-to-convert-any-web-template-into-a-wordpress-theme/" target="_blank">converting the final design to a wordpress theme</a>.

When I was satisfied I had a good enough design (for me at least) , I started looking for a place to host the site.

## Web Hosting with Servage
You never quite realize how many web hosting companies are out there until you do a search for one. And each one of those companies have there fair share of horror stories. So the best way to find a reliable hosting site is probably word of mouth. A friend of mine was hosting his website for the past two years on <a href="http://www.servage.net/?coupon=cust68241" target="_blank">Servage</a> and had no issues. I decided to give them a try.
<a href="http://www.servage.net/?coupon=cust68241" target="_blank"><img style="border-right-width: 0px; display: block; float: none; border-top-width: 0px; border-bottom-width: 0px; margin-left: auto; border-left-width: 0px; margin-right: auto" src="{{ site.baseurl }}/assets/servagebanner.gif" border="0" alt="Servage Web Hosting" width="644" height="86" /></a>
Servage offers the following

1. 750 GB of Space
2. 7500 GB Monthly Data Transfer
3. Unlimited emails
4. Free domain or domain transfer
5. Unlimited domains
6. Autoinstaller for the most popular web scripts

And many more features you can read about on their <a href="http://www.servage.net/?coupon=cust68241" target="_blank">website</a>.
Once I had my account, I used the one click autoinstaller feature to install wordpress and setup the mysql database. Wordpress version 2.6.2 was installed so I used the wordpress update feature to update the installation to version 2.7.  Simple an easy!

Finally, I exported my blog from the <a href="http://www.wordpress.com/" target="_blank">wordpress.com</a> site and imported into my <a href="http://asifhamza.com">http://asifhamza.com</a> site. All the content was now on a different server, but there were still a few issues that needed to be ironed out.

### The Case of the Missing Sidebars
For some reason my sidebars were not visible on the new site. After some fruitless googling I finally figured out the problem. My custom wordpress theme had a file called SideBar.php which describes how to render widget ready sidebars. The sidebars where showing up when I tested on my windows vista laptop since Windows filenames are not case-sensitive. But my site was hosted on Linux where filenames are case-sensitive. The wordpress theme engine was looking for sidebar.php not SideBar.php. A quick file rename solved that problem.

### The Case of the Missing Images
The second problem I found was that all the images were still linking back to the old site instead of the new even though they had been successfully imported. The old links were still embedded in the relevant posts. While I could have gone to each post and manually edit the urls, I used an <a href="http://www.velvetblues.com/web-development-blog/wordpress-plugin-update-urls/" target="_blank">Update Urls</a> from <a href="http://www.velvetblues.com" target="_blank">Velvet Blues</a>. 20 seconds later, the problems was solved.  As an added bonus, I found some helpful articles on blogging, wordpress and web design on their <a href="http://www.velvetblues.com/web-development-blog/wordpress-plugin-update-urls/" target="_blank">site</a>.

### The  Case of the Unco-operative Permalinks
The final problem I encountered was that my permalinks were no longer working. From experience I know that this is usually caused by the apache mod_rewrite plug-in not being enabled on the web server. 

A quick search on the Servage’s wiki and I found out that mod_rewrite could be enabled by enabling .htaccess support. All links were working within the hour.

Now that everything is up and running, I think it looks pretty good. Not matter what anyone else says! I spent the next week signing up for <a href="http://www.google.com/analytics/" target="_blank">Google analytics</a> and <a href="http://www.google.com/webmasters/tools" target="_blank">Google webmaster tools</a> and looking for nice plug-ins. I also ending up with a better appreciation of the power of CSS. Its amazing what you can do with xml and a stylesheet and I don’t think I’ve even scratched the surface.
