---
title: "Setting up Floodlight and FB Pixel tags / event calls"
description: This post is related to the gatsbyjs
date: '2019-05-17'
image: 'sunset.jpg'
---
## COH Project - Setting up Floodlight and FB Pixel tags / event calls
To do: Set up Flooglidhg and FB pixel tags / event calls

Troubleshooting
<p>
    - Ensure all data is received from client. This usually entails Tag Vendor, Tag Title, Code snippet, event desc (onClick, PageView, etc.) and URL where event should happen.
<p>
    - Create Floodlight tag. Setup data mappings. 
<p>
    - Setup DC settings in a lookup table. Ensure data layer variable is set, so you can map to that variable (ie, dc_settings) Scope to specific tag. Map the pathname to dc_settings. Look through code snippet and update the values (ie, coh200 locan0)
<p>
    - Set up Floodlight parameters. Map activity, activity_group, counting_method and event to a split method <b>See COH account for example</b>
<p>
    - Use jQuery onHandler exentension for button clicks. Trigger on mousedown. Link tracking event. Set activity_group, activity, event and counting_method to appropriate values (ie, coh200, impac0, conversion, standard)
<p>   
    - For the FB pixel PageViews, you can use data mappings. Map the pathname to the Tag Title, as provided by the client.
<p>
    - FB Pixel onClick events can be handled with jQuery onHandler extensions. Please see COH account extensions 317 for example. 


