## this file goes over the dissection of securly.com/blocked...

### the url by itself

https://www.securly.com/blocked?useremail=example@example.com&reason=domainblockedforuser&categoryid=000009&policyid=3&keyword=SG9tZXdvcms=&url=ZXhhbXBsZQ==
ill go over each part of this url one by one
 / https://www.securly.com/blocked (nothing to do here, just the base url)
<br>
<br>
<br>
 / ?useremail= (a query. without this query, the base url is shown differently (https://www.securly.com/blocked))<br><br>
 / ?reason= (a query. known states are below:<br>
    - domainblockedforuser<br>
      )<br><br>
 / ?categoryid= (a query. it shows on the blocked page. known states are below<br>
 ---- BL (the default? means 'blacklisted')<br>
 ---- 1 (Safe Search | smth bad)<br>
 ---- 2 (Youtube | bad video?)<br>
 ---- 3 (Safe Search, Youtube | youtube bad video searched?)<br>
 ---- 4 (Safe url | no idea, my only theory: never is used, just something like https://kahoot.it, which is listed as always allowed)<br>
 ---- 5 (Safe Search, Safe url | yea this one makes no sense if my theory is correct)<br>
 ---- 6 (Youtube, Safe url | idk)<br>
 ---- 7 (Safe search, Youtube, Safe url | idk)<br>
 ---- 8 (Innapropriate adult content | its not corn. its like gambling and stuff)<br>
 ---- 9 (Safe Search, Cxrnography | THIS one is corn)<br>
 ---- 10 (Youtube, Cxrnography | ngl, didnt think that could be on youtube in the first place)<br>
 ---- (there's more, but its mostly just repeats of others combined.)<br>
 ---- )<br><br>
 / ?policyid= (a query. known states are below<br>
 ---- 1 (High School Students)<br>
 ---- 2 (Middle School Students)<br>
 ---- 3 (Elementary School Students)<br>
 ---- 4 (All Staff)<br>
 ---- 5+ (Base/Default Policy)<br>
 ---- )<br><br>
 / ?keyword= (a query. this is a fun one, you can use this html (https://github.com/yesluckily/securly/blob/main/base64.html) page to translate text to base64 and vice versa. this is different than "?url=". ?keyword= is the word/reason the page got blocked, commonly used with search elements in websites.)<br><br>

 / ?url= (a query. this is also a fun one, you can use this html page (https://github.com/yesluckily/securly/blob/main/base64.html) to translate text to base64 and vice versa. this is different than "?keyword=". ?url= is the url that got blocked.)<br><br>
