---
title: "Trouble logging in through SSO"
description: This post is related to the gatsbyjs
date: '2019-05-18'
image: 'time.jpg'
---
## Ticket # 56414 - Trouble logging in through SSO
Problem: Client can't login to FreshDesk through with their SSO credentials

Troubleshooting
    - Make sure they are logging in through their portal or the SSO login portal located on the Tealium login pages

    - Are their SSO and Tealium IQ emails the same?

    - Is their TiQ profile set to the correct Primary Account? 

    - Have the client reset their browser's cache and cookies

    - Reset their user permission cache using custom code:https://community.tealiumiq.com/t5/QA/Permission-Cache-Updating-Users-and-Accounts-on-the-Fly-and/m-p/38
    - Delete user and re-add them (clears their cache)