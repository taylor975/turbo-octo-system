---
title: "Darryl Boyce is off the Christmas Card List"
date: 2023-11-04
---

I know what you're thinking:  Darryl Boyce of Summerside, PEI, date of birth 1984-08-04 is a nice guy who had a respectable 10-year pro hockey career that spanned four pro leagues and included 84 appearances in the best league in the world, _the National Hockey League_ - what did he ever do to you?

The answer is nothing; that Darryl Boyce is still on the Christmas card list, I can assure you.  No, the Darryl Boyce I'm speaking of is the one hailing from Lethbridge, Alberta, date of birth 1987-02-24 - _that_ Darryl Boyce is off the Christmas card list.  And while I'm sure he is probably a nice guy is well, his entry on National Hockey League's player database gave my computer fits when trying to pull his statistics from the NHL's public API.  You see, Darryl Boyce (Lethbridge, 1987) is a rare player in the NHL's database:  his biographical information stored at the _`/people`_ endpoint of the NHL API is [completely filled out](https://statsapi.web.nhl.com/api/v1/people/8473969), but his _`/stats`_ endpoint, which holds player statistics for a variety of leagues, is inexplicably empty.  This quirk in the database will cause any API pull request on Darryl's stats to throw an error - breaking any larger pull request loop that it may be a part of.

https://statsapi.web.nhl.com/api/v1/people/8473969/stats/?stats=yearByYear
