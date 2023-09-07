---
tags:
  - discord
---

Our current Discord bot is written in Golang and we use an additional bot called [[Whodis]] to verify that users are a member of the society when joining.

We plan to rewrite this bot in Python in the future, trimming away any unnecessary features (i.e the corona counter) and also heavily document it for future Sysadmins. In my opinion Python is the ideal language choice for the project as it is learned by all first year CS students and has an easy to use framework for interacting with the discord API