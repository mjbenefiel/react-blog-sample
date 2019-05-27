---
title: "on mousedown may be conflicting with another event; use click instead"
description: This post is related to the gatsbyjs
date: '2019-05-20'
image: 'sunset.jpg'
---
## COH Project - FB PageView event firing on all pages except for one
Problem: Mousedown should've been performing as expected but wasn't.

Troubleshooting
<p>
    - If a mousedown is conflicting with another event, try switching to onClick. This worked during an issue where mousedown should've been operating as you'd expect, but wasn't.
<p>
  


