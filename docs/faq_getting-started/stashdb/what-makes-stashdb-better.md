---
layout: default
title: What Makes StashDB Better?
nav_order: 7
parent: 'StashDB'
grand_parent: FAQ / Getting Started
---

# What Makes StashDB Better?

{: .important }
**Full integration with Stash and improved scene matching using various fingerprints (pHashes).**

---

StashDB is not the only source of much of its metadata. When filling out information in Stash, you will likely use multiple sources to cover various parts of your collection. Stash has a helpful [repository of scrapers](https://github.com/stashapp/CommunityScrapers){:target="_blank"} to assist with that. Each source will have its own strengths and weaknesses, just like StashDB. However, the main advantages of using StashDB over similar databases are:
1. **Full continuing integration with Stash.** Stash, Stash-Box, and StashDB are all part of the same shared project. They all enjoy the benefits of parallel development, always keeping each other in mind when creating or updating new features. Updating info in Stash from StashDB should be easier and more versatile than using other sources, just as updating StashDB from within Stash should become more convenient as well.
2. **The ability to match your files with scene entries on StashDB using hashes/fingerprints alone.** With the inclusion of [perceptual hashes]({{ site.baseurl }}/docs/faq_getting-started/stashdb/whats-a-phash/), even files of differing resolutions, encodes, or download sources will often be similar enough to still match with StashDB. In other words, your files and their hashes don't have to be exact matches with the fingerprints on StashDB. Stash will be able to find matches as long as your video _looks just similar enough_ to somebody else's fingerprint submission. This level of fuzzy matching makes our system much more reliable, flexible, and versatile than alternative approaches.
