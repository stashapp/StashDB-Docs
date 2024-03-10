---
layout: default
title: What's a pHash?
nav_order: 8
parent: 'StashDB'
grand_parent: FAQ / Getting Started
---

# What's a pHash?

{: .important }
**Perceptual hashes are generated from what a video looks like, allowing for more reliable scene matching with StashDB.**

---

[Perceptual hashes](https://hackerfactor.com/blog/index.php%3F/archives/432-Looks-Like-It.html){:target="_blank"} (pHashes) are one of the main reasons why we [recommend using StashDB]({{ site.baseurl }}/docs/faq_getting-started/stashdb/what-makes-stashdb-better/) with Stash. pHashes are used to match your video files with scene entries on StashDB. Even files of differing resolutions, encodes, or download sources will often be similar enough to still match with StashDB. In other words, your files and their hashes don't have to be exact matches with the fingerprints on StashDB. Stash will be able to find matches as long as your video _looks just similar enough_ to somebody else's fingerprint submission. This level of fuzzy matching makes our system much more reliable, flexible, and versatile than alternative approaches. pHashes can also be used in Stash to detect duplicate files in your library, using the "Scene Duplicate Checker" in the "Tools" tab of the Settings page.

pHashes are not generated in Stash by default, so you will need to create them yourself. They may be generated during a Scan by activating the switch next to "Generate perceptual hashes" or through the Generate task (in the "Tasks" tab of the Settings page or the "Generate..." option with individual scenes selected) next to "Perceptual hashes (for deduplication)". These may be submitted to existing scenes on StashDB along with other fingerprints using the [Scene Tagger]({{ site.baseurl }}/docs/faq_getting-started/stashdb/using-stashdb/) and will be included automatically when [submitting new scenes via draft]({{ site.baseurl }}/docs/faq_getting-started/stashdb/using-stashdb/).
