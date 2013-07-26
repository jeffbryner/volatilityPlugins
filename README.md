volatilityPlugins
=================

My volatility Plugins. 

twitter.py 

Extracts twitter html and json data from a memory image. 

sample session: 
vol.py -f bryner/memimages/win7chromefbtwitter  --profile=Win7SP1x64  twitter

Volatile Systems Volatility Framework 2.3_alpha
searching for browser processes...
found browser pid: 2780, chrome.exe
examining 86639978 bytes
twitter cookie found for userid:61387084
found browser pid: 2288, chrome.exe
examining 89884416 bytes
profile: @p0wnlabs,     3,536 Tweets     933 Following     1,171 Followers
8:39 PM - 25 Jul 13 (21s)       @kateesackhoff  Katee Sackhoff
                Explain this...! I have 3 dogs, 1 is 7months old, I've never been allergic to a dog in my whole (cont) http://tl.gd/mbn8j5

facebook.py 

Extracts facebook html and json data from a memory image

vol.py -f bryner/memimages/win7chromefbtwitter  --profile=Win7SP1x64 facebook

Volatile Systems Volatility Framework 2.3_alpha
searching for browser processes...
found browser pid: 2496, chrome.exe
examining 86980777 bytes
found browser pid: 2576, chrome.exe
examining 74650769 bytes
found browser pid: 1364, chrome.exe
examining 97578571 bytes
Likely facebook user json structure: {"id":"1421688057","name":"Jeff Bryner","firstName":"Jeff","vanity":"jeff.a.bryner","thumbSrc":"https://profile-a-pao.xx.fbcdn.net/hprofile-prn1/s32x32/50109_1421688057_6617527_q.jpg","uri":"https://www.facebook.com/jeff.a.bryner","gender":2,"type":"user","is_friend":false,"social_snippets":null}
Date: Thursday, July 25, 2013 at 8:01pm about an hour ago in Las Vegas, NV url: https://www.facebook.com/LanceJames/posts/10201006553878572
        Author: Lance James             https://www.facebook.com/LanceJames?hc_location=stream
                Text: with Jaleesa Stringfellow at McCarran International Airport - Las Vegas, NV.
                img: https://profile-b-pao.xx.fbcdn.net/hprofile-prn2/1076381_1608857704_1305884837_q.jpg
                Text: Landed
etc...

Both plugins also accept a -p PID argument if you want to specify a specific browser process ID instead of having it search any browser process it finds.


