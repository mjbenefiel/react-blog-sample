---
title: "Tag not firing on site, but firing locally"
description: This post is related to the gatsbyjs
date: '2019-05-18'
image: 'sunset.jpg'
---
## Ticket # 56370 (partially complete) - Tag not firing on site, but firing locally
Problem: First part of this problem is the client's 4cite tag is not firing on their site; however, it's firing on my localhost.

Troubleshooting
<p>
    - Check to see if the tag is set to "all pages" load rules, and if it's bundled.
        - To check if "all pages" are bundled, click save/publish > configure publish settings > Bundle tags loading on all pages
<p>
    - If it's bundled, you can check to see if the tag is firing in the utag.js, by going to the sources tab in DevTools
<p>
    - If you step through the code (checking track/view, etc) and values are being returned, then it's most likely a problem with the client's web configurations. IT or the vendor will need to help them at that point. Further, the base URL should fire after you step through the code completely. You can also try a manual fire by placing utag.view(utag_data, null [uid]) into the console.

There will be more to document on this tag, but this is the first step to resolving the issue. 