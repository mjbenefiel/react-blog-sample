---
title: "Trouble logging in through SSO"
description: This post is related to the gatsbyjsa
date: '2019-05-14'
image: 'time.jpg'
---
## Ticket # 56414 - Trouble logging in through SSO
Problem: Client can't login to FreshDesk through with their SSO credentials

Troubleshooting
<p>
    - Make sure they are logging in through their portal or the SSO login portal located on the Tealium login pages
<p>
    - Are their SSO and Tealium IQ emails the same?
<p>
    - Is their TiQ profile set to the correct Primary Account? 
<p>
    - Have the client reset their browser's cache and cookies
<p>
    - Reset their user permission cache using custom code:https://community.tealiumiq.com/t5/QA/Permission-Cache-Updating-Users-and-Accounts-on-the-Fly-and/m-p/38
<p>
    - Delete user and re-add them (clears their cache)