---
title: "FB PageView event firing on all pages except for one"
description: This post is related to the gatsbyjs
date: '2019-05-18'
image: 'sunset.jpg'
---
## COH Project - FB PageView event firing on all pages except for one
Problem: FB PageView event firing on all pages except for one

Troubleshooting
<p>
    - Verify if there is a tag hardcoded on the site. If so, that is conflicting with the Tealium FB Pixel Tag, due to the hardcoded site being read first by compiler/engine/browser
<p>
    - Verify if client is using latest version of tag by using tag status checker in TiQ. 
<p>
    - If not running latest version, jump to own account and activate the latest version of a tag. Run the tag in your sandbox. Copy and paste the latest utag.xx.js file into VScode for manipulation. 
<p>
    - To inject the new tag into the site via Charles, there are several steps that need to be taken.
<p>
    - Map Local the request URL of the tag that's being fired in Networks tab. Set the Query string to *
<p>   
    - In the latest version of your own tag, you will need to replace all instances of your tag UID with the UID of the tag running on the client's site. You will also need to update the account name at the bottom (ie, coh.main)
<p>
    - Next, go to TiQ and open up the source code of the client's outdated tag. You can do this by clicking/opening the tag row and then clicking on the UID. From there, you will need to copy/paste the u.map object and u.extend IIFE into your version that's being locally hosted. Make sure to leave come custom comments on top so you can ID if the tag is being mapped correctly. 
<p>
    - In Charles, map that file to the hostname declared in Charles. At this point, you should see the updated tag running in the sources tab. If it's not being picked up by FB pixel helper, or in the networks tab, then the client will most likely need to remove the hardcoded tag. 


