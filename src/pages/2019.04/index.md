---
title: "Testing lookup table outputs with no staging site"
description: This post is related to the gatsbyjs
date: '2019-05-16'
image: 'sunset.jpg'
---
## Implementation Project - Servus - Testing lookup table outputs with no staging site
To do: Update lookup table with new values, and validate on site using DevTools. No staging site available.

Troubleshooting
<p>
    - Verify client has provided all necessary data. Generally this will be the URL, activity and activity group if you're working with DoubleClick Floodlight
<p>
    - Merge all data so you can import it into TiQ lookup table. Can be accomplished in various ways. Make sure to use concatanate to achieve a single row of data. Text to columns can be helpful to quickly remove unnecessary characters.
<p>
    - After import is successful, you will need to proxy in through Charles using Local Map. 
<p>
    - First step is to copy and paste the page's source code into VSCode
<p>
    - Proxy > SSL Proxy Settings > Make sure *:* and tags.tiqcdn.com are enabled
<p>   
    - Tools > Map Local > Add Host > Copy and paste URL into host and press tab. Make sure query is set to *
<p>
    - Local Path > Map the file you have the source code located in
<p>
    - At this point, Charles should be mapping correctly and you can validate the site's information as if it were running as you have setup, without actually changing anything from the development side. 
<p>
    - Testing values in lookup tables involves going to network tab and navigating to appropriate instance and checking the url request.

