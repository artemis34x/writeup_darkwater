# Dark Water write up

**Welcome to Dark Waters, a scenario that allows you to take on the role of Investigative Journalist Alec Wolfe as he uncovers deadly secrets about a small town in Pennsylvania.**

Through Alec, you will experience first-hand what it's like to collect, analyze, and verify a breaking news piece for a newspaper. This scenario is designed to challenge and encourage you throughout the story to implement Open Source Intelligence and digital investigation techniques including:

1. Social media analysis
2. Visually extracting key data points from an image or video
3. Applying tools, methods, and resources to answer contextual questions to uncover the truth.

When you have completed this scenario you should be comfortable applying tools and methodologies frequently used in digital investigations including journalism. You learn to pivot from key data points and collect information used to answer investigative questions.

---
## Strange Letter
![strange letter](img/Strange_Letter.jpg)
![letter P](img/Letter_P.jpg)

We are starting with 2 pictures addressed to our journalist Alec Wolfe from "P", an unknown sender.
We have a few information already:
- We know where to investigate, Glen Rock PA
- There is something going on with the water

---

## Welcome to Glen Rock, PA!
In this section, we have a video showing Alec driving to the bar of Glen Rock. 

---

## At The Bar
Arriving at the bar, Alec meet Lisa the barman and rent a room in her bar for his stay.

---

## The Protestor
Outside of the bar, Alec notices a young woman on the sitting in the sidewalk with a cardboard sign.
While talking to her, we can get some information about the town:
- Her family had been in the town for a while
- Her mother's great-grandfather bought the land of Glen Rock in 1837
- Her mother's great-gradfather refused to give the land to the GRPC plant

---

## GRPC: The Company That Cares About Nature
This section is showing a promotional video for GRPC and how they protect and care about the nature of the town.
Additionnaly we have their website [GRPC](https://www.kaseportal.com/grpc). 

---

## Getting to know the town

**Q1 - What is the name of the protestor's relative that was the first to own land on what is now Glen Rock?**

![William Heathcote](img/Q1.png)

For this question, I could find the anwser by looking at the history of Glen Rock on [Wikipedia](https://en.wikipedia.org/wiki/Glen_Rock,_Pennsylvania).

> 🚩Flag: *William Heathcote*

**Q2 - What is the name of the main Railroad through town?**

![Railroad](img/Q2.png)

I used the same [Wikipedia](https://en.wikipedia.org/wiki/Glen_Rock,_Pennsylvania) page to find the anwser. If I try to search an element on the page by typing "Rail", I found the flag.

![Maps](img/rail.png)

To confirm my finding, I can use google maps to make sure this is the correct railroad.

> 🚩Flag: *Northern Central Railway*

**Q3 - On the side of the local library, what does the third part of the mural say?**

I could find the local library by searching on Google maps.

![Library](img/library.png)

I found the "[Arthur Hufnagel Public Library of Glen Rock](https://goo.gl/maps/m69N9PPFZXpNoNDz7?coh=178572&entry=tt)", but after trying with Street View I couldn't get a closer look on the mural painting.

![Mural](img/mural.png)

After looking in the pictures posted in the library reviews, I found a picture in front of the mural I could use.

![Mural Front](img/Q3.png)
![Mural Close](img/Q3close.png)

I could read the writing of the mural using this picture. After trying the flag "FIRST NATIONAL BANK", it doesn't work so I though that might be a typo or a case sensitive flag.

> 🚩Flag: *First National Bank*
  
**Q4 - Which female artist donated her pastel work "under the rainbow" to the library?**

I was stuck on this one because I couldn't find the pastel work. But after using Google dorking, I found a [newspaper](https://issuu.com/engleprintingandpublishing/docs/ccs_102319) talking about a library diplaying artwork. After reading the article, I was able to get the flag.

![Article](img/Q4.png)

> 🚩Flag: *Maryanne Smith*

**Q5 - What is the street name of Maryanne’s studio?**

A good Google search can flag this one. After searching for "Maryanne Smith studio glen rock", I get a [Linkedin](https://www.linkedin.com/in/maryanne-smith-0a6bb757) profile and a website selling [art](https://auctions.slamquest.org/SLA-55-Altay-Argali-Painting-by-Maryanne-Smith_i35406483) for auction.

Maryanne studio location can be found in the item description.

![Art](img/Q5.png)

> 🚩Flag: *Ronald Street*

**Q6 - Where was this taken in town?**

![tag](img/tag.png)

I could find the place by reversing it on Google image, it was linked to a [Facebook](https://www.facebook.com/RuinsHall/)

![Ruins](img/Q6.png)

> 🚩Flag: *Ruins Hall*

**Q7 - The protester was attending an event there on June 8th 2018 what was it?**

This one was a little bit complicated for me because I was looking for any post or article at this date.

But after trying to search on the ruins hall Facebook page with a filter on the date, I still couldn't get anything.

![Filter](img/filter.png)

I got a result after searching for "June" in the result of the filter.
From here, I found the flag in the post description.

![movie night](img/Q7.png)

> 🚩Flag: *Movie Night*

**Q8 - Which movie was shown at the event?**

The answer of the question was also in the post but under it was a poll where we could choose for the movie.

The flag here is the most voted movie.

![Movie](img/Q8.png)

> 🚩Flag: *Back To The Future*

**Q9 - What was the high temp on that day in Celsius(Only one decimal point is needed)?**

A quick search on Google and a website that archive the weather data helped me to find the flag.

![weather](img/Q9.png)

> 🚩Flag: *28*

---

## Cocktail Party

We have a flyer in this section inviting us to a cocktail party organized by the GRPC.

![Flyer](img/GRPC_AnnivFlyer.jpg)

---

## Party Recon

We find some important personnality of the town at the party, like the the local politician and the CEO's son of GRPC.

---

## Eavesdrop

We overhear a conversation between 2 guards in front of the line for the party. They are talking about some kind of drop and side hustle to make money on the side. 

Sadly they don't allow us to go in because we are not on the list.

---

## Text To George Hammond

We are texting our boss, George Hammond, because we couldn't get inside the party, it was too crowded.

## The Employees

**Q10 - Who created this flyer?**

For this flag, I used the metadata of the flyer we got from earlier and from the author of the file, I got the flag.

![Author](img/Q10.png)

> 🚩Flag: *Patti Stanton*

**Q11 - What is Patti's favorite thing to do?**

There is only one place where we can see any information about her: the company website we saw earlier.

https://www.kaseportal.com/grpc

![Staycations](img/Q11.png)

> 🚩Flag: *Staycations*

**Q12 - What is Patti's home SSID?**

For this question, I didn't even know that OSINT on SSID or WiFi was possible so look it up on Google for the first time. And I found a website showing how to do OSINT on SSID using the website : https://wigle.net .

But even with the tools to find the flag, I couldn't find where to start with only a few information:
- her name "Patti Stanton"
- where she works "GRPC" and her job here "Event Management"
- where she lives maybe "Glen Rock"?
- she loves "staycation"

Just to make sure she wasn't a real person, I checked on Google in case I find something else but nothing here. Since the website with the Wifi map have a search tool integrated, I used the information we had on her supposing she modified her SSID to her name or something easy to remember.
The search tool also had the possibility to search with wildcards "%" so it might be easier to the SSID that way.

![search](img/search.png)

Based on that supposition, I started with her name  and the location "Glen Rock" with wildcards around it, found nothing for it.

![location](img/glen.png)

Staying in Glen Rock, I searched for a company building or address if I could find an address but nothing here too.

But after looking for "staycation", it finds 1 Wifi router in Glen Rock.

![Q12](img/Q12.png)

> 🚩Flag: *staycation Wifi*

**Q13 - What is the BSSID?**

After finding her SSID, I find that the website store a few information about that router.

![Q13](img/Q13.png)

> 🚩Flag: *3C:7A:8A:93:D2:5E*

**Q14 - What year was this BSSID first seen?**

> 🚩Flag: *2021*

**Q15 - What is the vendor of this device?**

For this question, I know that every device has its vendor name if we search on MAC address database.

https://mac.lc/address/3C-7A-8A

![Q15](img/Q15.png)

> 🚩Flag: *ARRIS Group*

**Q16 - What is the parent company of Arris Group Inc?**

This question was a bit trickier than I thought because if we just put the parent company written on wikipedia, it doesn't work.

![com](img/com.png)

But if we just look at the parent company before the current one bought it, we have another parent company.

![Q16](img/Q16.png)

> 🚩Flag: *Arris International Limited*

---

## Campaign funding

**Q17 - How much money has GRPC donated to Alexander Ross?**

This question take us back to the beginning where they give us the company website. Next to the the cocktail party flyer, we can see a few information about the company news.

![Q17](img/Q17.png)

After reading them, we find the information about Alexander Ross campaign.

> 🚩Flag: *1,214,000*

**Q18 - What is the GRPC campaign phone number for Alexander Ross?**

When we had the website at the beginning, I already read everything on it to make sure I wasn't missing something. So the phone number was at the bottom of the page associated with Alexander Ross name.

![Q18](img/Q18.png)

> 🚩Flag: *(931) 532-0554*

**Q19 - How much did Glen Rock Paper Company spend on PR services in 2022?**

First, I thought that PR meant "press release" but after looking at the annual report for shareholders, I couldn't find anything that matches.

I ended up reading the whole report and found Public Relations Fees.

![Q19](img/Q19.png)

> 🚩Flag: *11,576*

---

## Taking a water sample

We are taking a water sample from river and we are sending it to make test on it.

---

## The locals

Going back to the bar, we have a confrontation with the locals because we are not from the town and they are suspicions about us.

---

## Who is P?

We get new material from the discussion we have with Lisa the bartender, she revealed that the room we were sleeping in was her brother's bedroom. And that his name was Peter with his tragic story. So we can already link him with the "unknown sender" of the letter. She also gave us the intel gather by the detective investigation on his death.

---

## Voicemail from Peter

We learn here that there is a photo that might be useful for later. Lisa is holding on it.

---

## Calling the lab

After calling the lab, we thought that we could get some information about our water test but we ended up learning that someone cancelled the test with a fake email to the lab.

---

## Lab test cancelled

![cancelled](img/cancellation.png)

If we look at the email that sent the message, it's clear that someone is trying to stop us from testing the water. We got the e-mail address of the person at least.

'rockthesocks1982@fastmail.com'

---

## Rock the socks

**Q20 - What is the full name of the owner of this email address?**

I tried to search for the email address on google in case I could find a hint, nothing here.

![mail](img/mail.png)

Maybe trying with the first part of the email address: "rockthesocks1982".Using the tool "[blackbird](https://blackbird-osint.herokuapp.com/)", I got 2 usable results. 

![blackbird](img/black.png)

The first one is a Facebook account but I couldn't get an access.

![facebook](img/face.png)

The second one is a Reddit account, I could see that he posted some comments.

![reddit](img/reddit.png)

Following the steam link, we find a steam account.
We still stuck but at least the hint is good because the user is from Pennsylvania, the state of **Glenn Rock**.

![steam](img/steam.png)

I got stuck with this steam account for a long time until I decided to try everything I could on the website.
So I ended up searching for the username "sloppyfpsgame1982" on the community page. After finding the account again, it also give us a name that looks like a real name.

https://steamcommunity.com/search/users/#text=sloppyfpsgamer1982

![john](img/john.png)

The name is almost complete, we just need the last name of "John". With that hint in mind, I oriented my search in 2 ways:
- the first one with a simple google search
- the second one with the Facebook result we got from "Blackbird"

The first one is not working or I didn't searched correctly.

The second one is to search for "John B" on Facebook because we had a match on the username "rockthesocks1982" but we couldn't get a proper access.
Using all the information we know about "John B", we can search with a filter like the location.

![filter](img/name.png)
![Q20](img/Q20.png)

> 🚩Flag: *John Banks*

**Q21 - What year was he born?**

We could guess the answer based on the username used on his social media account.

> 🚩Flag: *1982*

**Q22 - Which city is John from?**

From here, we can use his Facebook account to answer but the place is not explicitly specified. However, we can also guess with where he come from.

![Q22](img/Q22.png)

> 🚩Flag: *Las Vegas*

---

 ## Voicemail

 We have a voice message from our boss that gives us a post on a reddit conspiracy group.

 ![resistance](img/resistance.png)

 ---

## What is the cache?

**Q23 - What is the name of the cache?**

![secret](img/code.png)

This is the first time I see this kind of secret code if there one here. :)

Since this looks like UTF8 encoded it might means something if we translate it to ASCII encoding for example. I tried to find something on the tool "dcode".

After a while, I couldn't find anything so I started searching on Google and finally found something that looks like our secret code: "webdings fonts".

https://www.dcode.fr/webdings-font

![web](img/web.png)

The message translate to : *Incoming cache drop.Sloppyfpsgamer*

If it talks about a cache it might be something on the website "Geocaching.com". Since we have no idea for what to look for, I guess we could try to look for a cache in Glen Rock but there was nothing obvious that I could find. However, after trying to find a way to search for a player instead of a cache, I found a match for the username "Sloppyfpsgamer".

To find the "find Another player" option, I had to go on the dashboard of my profile > find another player and we find the search bar.

![player](img/player.png)

![sloppy](img/sloppy.png)

We find in the tab Geocaches an owned cache.

![cache](img/cache.png)

We finally find the name of the cache in his cache.

![Q23](img/recon.png)

> 🚩Flag: *GRPC recon*

**Q24 - What are the coordinates of the cache?**

The answer could be found in the description of the cache.

![coordinates](img/coordinate.png)

*Note: the flag have a different syntax when copied from the first coordinate. You need to copy from the edit option or rewrite it manually.*

> 🚩Flag: *N 39° 48.185 W 076° 53.772*

**Q25 - What did the encrypted text say that was posted on the conspiracy forum?**

I already have decypted the message above for this one.

> 🚩Flag: *Incoming cache drop.Sloppyfpsgamer*

---

## Finding the cache

Going to the cache, we find a small cache with a paper inside. There is a message written on it but it looks like encoded again.

![rot13](img/rot13.jpg)

---

## Interressing communication techniques

**Q26 - What does the text translate to?**

When looking at the description of the cache, to find any hints I already noticed the "additional hints" section which contains an encryption system.

The message on the paper looks a lot like this encyption, I tried it. And we obtain the message decrypted.

![keys](img/key.png)

*Note: the encryption was rot13 I saw it later.*

> 🚩Flag: *Next flyover: Lake Marburg*

**Q26 - What does N1822H reference?**

The number looked like a reference to a plane number so to make sure that was the correct guess, I just checked that on Google and it was correct.

> 🚩Flag: *plane*

**Q27 - What type of aircraft is N1822H?**

Since the plane could be found online, I could easily get his model but I had make some changes in the flag because it didn't want the full name.

![planes](img/plane.png)

> 🚩Flag: *Piper PA-28-181*

---

## Getting some flight data

We are asking our boss to give us some information about the flight N1822H and he sends back a file.

https://kasescenarios.com/FlightAware_N1822H_KFDK_KFDK_20230108.zip

![flight data](img/data.png)

---

## Come fly with me

**Q28 - Which airport did this aircraft fly out of on January 8th 2023?**

The zip file we got above could be imported into Google earth pro, and we obtained the whole flight data from the 8th of January 2023.

![map](img/map.png)

The view of the flight path from above show us where he started and ended.

> 🚩Flag: *KFDK Airport*

**Q29 - Which lake did the plane fly over on January the 8th?**

On Google Earth pro, I could easily put a filter to look for lake.

![layers](img/layers.png)

We see on outlined lake and it was the lake where the cache was hidden.

![lake](img/lake.png)

If we look closer to the lake we have its name and it also confirm the hidden message in rot13 earlier: *Next flyover: Lake Marburg*

> 🚩Flag: *Lake Marburg*

---

## Threatening phone call

We got a call from an unknown number threatening us.

![call](img/call.png)

---

## Unknow phone number

**Q30 - Who is the owner of the phone number?**

This question was very complex because a simple search on google or some phone database could get us the answer. I had no idea where to look for after using the only way I knew to find the flag. 

After searching for a while, I decided to look back and look in the material we got so far. The only thing I didn't explore was "John Banks" Facebook profile in depth. So I started reading every single post he made, and finally found the number but not associated with the name of the owner yet.

![banks](img/banks.png)

I need to look for the admin assistant in GRPC.
I went to the company website and look in the employee of the month. The owner was here.

![admin](img/admin.png)

> 🚩Flag: *Aleigha Brooks*

---

## Voicemail from Lisa

Her voicemail mention the picture Peter told her to keep. She found out that the picture had a writting on the back of it.

![peter1](img/peter1.jpg)

![peter2](img/peter2.jpg)

---

## Image exploration

**Q31 - 0x**

Since my study is cybersecurity, I just understood that it was some kind if hexadecimal code. I started looking for the username on the picture since I could't explore the picture itself, I had no idea where to look for an old boat.

Google result for "Hoagie215" was not helpful. But after typing it in another search engine just in case, I found a good result on Yandex, a NFT page on "Opensea".

![open](img/open.png)

This make so much sense now because the small boat drawing was the Opensea logo. And the hexa is the Etherum wallet.

![ether](img/ether.png)

> 🚩Flag: *0x446eEB480516B7824C4D938740A5a410CA0cdB34*

**Q32 - Image 1**

This is the same question as before, no context just "image 1". But saw that the Opensea account had 3 NFT images, even if we know that we still have no clue. So I tried to find something hidden with steganography, no results here.

![robots](img/robot.png)

![robot1](img/cool1.png)

Nothing in the metadata too. It was also my first time with image analysis so I googled it to see if tools existed, and I found 2 tools on a website: https://www.osintessentials.com/image-analysis.

- https://fotoforensics.com/ this tool showed some kind of writting in the robot but it was not clear enought. But it gave me a hint to start with.

![cool12](img/cool12.png)

- https://29a.ch/photo-forensics/#forensic-magnifier this tool had way more options than the first one. I tried every options and played with the parameters to find the hidden text.

Using the luminance gradient with the max intensity, I can almost clearly see the text.

![Q32](img/Q32.png)

> 🚩Flag: *15.03.2023*

**Q33 - Image 2**

Same here no context and I guess it's on the "cool robot 2" NFT.

![cool2](img/cool2.jpg)

Using the same option as before we have a name now.

![Q33](img/cool21.png)

> 🚩Flag: *LU YANG SHUN*

**Q34 - Image 3**

Same option, we obtain coordinates.

![cool3](img/cool3.jpg)

![Q34](img/Q34.png)

*Note: the flag syntax here changed a bit because if we put it like the picture, it won't work. The coordinates are good but we need to replace the dot in the middle by a coma.*

> 🚩Flag: *39.264969, -76.598633*

---

## Final

And that's it for the Dark waters, I never thought I would complete it hopefully some friends helped me for some of the hardest questions XD.
