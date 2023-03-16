# OSINT mix

A stripped index of tools, I only add those that I feel comfortable with and that I think work perfectly.
Some of the services indicated are unfortunately subject to payment, these will be indicated with a big "NON_FREE" flag

## Table of Contents

- [Username](#username)
- [Email](#email)
- [Telephone Numbers](#telephone-numbers)
- [Meta](#meta)
- [Telegram](#telegram)
- [GeoIntelligence](#geointelligence)
- [Darknet](#darknet)
- [Face Search](#face-search)
- [Image Search](#image-search)
- [Cryptocurrencies](#cryptocurrencies)
- [Malware Analysis](#malware-analysis)
- [Threat Intelligence](#threat-intelligence)
- [Transportation](#transportation)
- [EXIF Data](#exif-data)
- [Automation&study](#automation&study)


----
## Username

- [Maigret](https://github.com/soxoj/maigret) -  My favorite username search tool, in addition to searching many social networks, also allows you to create reports in various formats
- [WhatsMyName](https://whatsmyname.app/) -In my opinion the web version works better, but if you want you can download the repository from github
- [Literally google](https://www.google.com/search?q=it%27s+easy). It's amazing how sometimes a google search with the username between "" is effective to find more information.

## Email
- [haveIBeenPwned?](https://haveibeenpwned.com/) this is easy, we all know it
- [Intelx](https://intelx.io/) NON_FREE very powerful tool to search for emails, telephone numbers, cryptocurrency transactions and much more inside various leaks and dumps. It costs? Very very much. But you can use it with partially limited functions by making a new free account for a few days/weeks. It does not require corporate email
- Google dorks: 
```intext:"@example.com" inurl:facebook.com```
```intext:"@example.com" inurl:site[dot]stuff```
```intext:"john@123"```
- [Email Reputation](emailrep.io) → usage: ```curl -s emailrep.io/[TARGET-EMAIL]```
- [The Harvester](https://github.com/laramies/theHarvester) OSINT gathering tool for email reconnaissance.
- [h8mail](https://github.com/khast3x/h8mail) An awesome tool that collects information from various sources about data leaks, dumps, and more. You can use h8mail with various API: 
---
| Service | Functions | Status |
|-|-|-|
| [HaveIBeenPwned(v3)](https://haveibeenpwned.com/) | Number of email breaches | :white_check_mark: :key: |
| [HaveIBeenPwned Pastes(v3)](https://haveibeenpwned.com/Pastes) | URLs of text files mentioning targets | :white_check_mark: :key: |
| [Hunter.io](https://hunter.io/) - Public | Number of related emails | :white_check_mark: |
| [Hunter.io](https://hunter.io/) - Service (free tier) | Cleartext related emails, Chasing | :white_check_mark: :key: |
| [Snusbase](https://api.snusbase.com/admin/purchase) - Service | Cleartext passwords, hashs and salts, usernames, IPs - Fast :zap: | :white_check_mark: :key: |
| [Leak-Lookup](https://leak-lookup.com/) - Public | Number of search-able breach results | :white_check_mark: (:key:) |
| [Leak-Lookup](https://leak-lookup.com/) - Service | Cleartext passwords, hashs and salts, usernames, IPs, domain | :white_check_mark: :key: |
| [Emailrep.io](https://emailrep.io/) - Service (free) | Last seen in breaches, social media profiles | :white_check_mark: :key: |
| [scylla.so](https://scylla.so/) - Service (free) | Cleartext passwords, hashs and salts, usernames, IPs, domain | :construction: |
| [Dehashed.com](https://dehashed.com/) - Service | Cleartext passwords, hashs and salts, usernames, IPs, domain | :white_check_mark: :key: |
| [IntelX.io](https://intelx.io/signup) - Service (free trial) | Cleartext passwords, hashs and salts, usernames, IPs, domain, Bitcoin Wallets, IBAN | :white_check_mark: :key: |
| :new: [Breachdirectory.org](https://breachdirectory.org) - Service (free) | Cleartext passwords, hashs and salts, usernames, domain | :construction: :key: |

*:key: - API key required*  
---
----
## Telephone Numbers
- [Google!](www.google.com) → some example ```"COUNTRYCODE\sNUMBER"``` ```+1 0000000000``` ```00000000```
- Telegram → add the number to your telegram contacts, then open the profile and delete the contact to see the nickname
- HaveIBeenPwned → add the number with country code withoud "+"
- [Phoneinfoga](https://github.com/sundowndev/phoneinfoga) 
- [whoisxmlapi](https://tools.whoisxmlapi.com) → NON_FREE but you can make a test account with 500 credits, no business mail required
`There are other tools but you risk going outside the OSINT scope`
----
## Meta
What would you like to find on meta?
Well remember that the id of a facebook account can be found by exploring the source of the profile, even without being logged in, it is generally the value of owner_id=[id]; profile_id=[id]. I don't know if you want to make a script to collect ids, in my opinion it goes outside the OSINT methods
- [Osintgram](https://github.com/Datalux/Osintgram) → powerful and functional, collect various public information from instagram profiles. Requires an account 
- [well...Whatsapp?](https://play.google.com/store/apps/details?id=com.zzttz.whatsdog) NON_FREE
----

## Telegram
- [Intelx](https://intelx.io/tools?tab=telegram)
- [lyzem](https://lyzem.com/)
- [username hystory](t.me/SangMataInfo_bot) → sangmata info bot
- [Graph messenger](https://www.graphmessenger.com/)
----
## GeoIntelligence
- [3Dcity](https://www.3dcitydb.org/) NON_FREE
- [Google cloud vision API](https://cloud.google.com/vision) NON_FREE
- [a VERY interesting paper](https://www.crcv.ucf.edu/wp-content/uploads/2019/10/Zamir_ECCV_2010.pdf)
- [for the nerdiest nerds](http://3drepresentation.stanford.edu/)
----
## Darknet
- [Ransomwatch](https://ransomwatch.telemetry.ltd/#/INDEX)
- [OnionSearch](https://github.com/megadose/OnionSearch)
- [Ahimia Search Engine](https://ahmia.fi/) 
- [OnionScan](https://github.com/s-rah/onionscan)
- [Hunchly](https://www.hunch.ly/) NON_FREE
----
## Face-Search
- [PimEyes](https://pimeyes.com/) Currently the best face finder I've tried, NON_FREE
- [face++](https://www.faceplusplus.com/) Cool for face comparisons
----
## Image-Search
- [Tineye](https://tineye.com/)
- every reverse image search of google, yandex, bing etc.

----

## Cryptocurrencies
- [orbit](https://github.com/s0md3v/Orbit) Crawling in blockchain
- [intelx](https://intelx.io/)

----
## Malware-Analysis
- [VirusTotal](https://www.virustotal.com/gui/)
- [AnyRun](https://any.run/)

----
## Threat-intelligence
- [Kaspersky Cybermap](https://cybermap.kaspersky.com/)
- [Awesome collection](https://github.com/hslatman/awesome-threat-intelligence) From https://github.com/hslatman 
----

## Transportation
- [Flightradar](https://www.flightradar24.com/)
- [VesselTracker](https://www.vesseltracker.com/)
- [Openrail](https://www.openrailwaymap.org/)
- [Satellite Tracking](https://www.n2yo.com/)

----
## Exif-data
- [exiftool](https://exiftool.org/)
----
## Automation&study
I recommend that you study the hackthebox academy module over and over again - OSINT: CORPORATE RECON
↓↓↓
https://academy.hackthebox.com/module/details/28
