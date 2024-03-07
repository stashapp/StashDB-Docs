---
layout: default
title: Using StashDB
nav_order: 3
parent: 'StashDB'
grand_parent: FAQ / Getting Started
---

# Using StashDB

{: .important }
**Tagger Views are recommended for pulling info from StashDB, Identify task is faster but less accurate.**

---

The recommended method for pulling information from StashDB into your local Stash is through the Tagger view. The Tagger can be found on both the Scenes page and the Performers page by clicking on the double-label icon on the far right end of the toolbar near the top of the webpage.

With the [Scene Tagger](https://docs.stashapp.cc/in-app-manual/tagger/){:target="_blank"}, you can match your scenes with StashDB entries by keyword or fingerprint, save that information to your scene including a link to StashDB called the StashID, and submit your fingerprints back to StashDB to help other users match their own scenes. Be sure to check out the "Scrape All" button (limited to one page at a time), the green checkmarks to customize which fields to overwrite, and the gear icon for additional settings. If you've already found your scene's entry on StashDB, you can paste the [StashID]({{ site.baseurl }}/docs/faq_getting-started/stashdb/whats-a-stashid/) directly into the "Query" field to ensure an accurate match. New users may find our [Guide to Scraping](https://docs.stashapp.cc/beginner-guides/guide-to-scraping/){:target="_blank"} helpful, featuring a detailed step-by-step walkthrough with screenshots. Stash's in-app manual also has a shorter rundown of its features, found by clicking the "?" icon in the top right corner of Stash or at [this link here](https://github.com/stashapp/stash/blob/develop/ui/v2.5/src/docs/en/Manual/Tagger.md){:target="_blank"}.

The Performer Tagger works similarly. Don't miss the "Batch Add Performers" and "Batch Update Performers" buttons on the top right, with a "Show Configuration" link on the opposite side. You can still paste the [StashID]({{ site.baseurl }}/docs/faq_getting-started/stashdb/whats-a-stashid/) directly into the search field if you've found the correct performer entry on StashDB already. Individual fields can be turned on and off for each scrape as well.

The [Identify](https://docs.stashapp.cc/in-app-manual/tasks/identify/){:target="_blank"} task can also pull scene info from StashDB, but it is not recommended for new users at this time. This is considered an advanced feature of Stash and will be hidden behind the "Advanced Mode" toggle in the settings page. You can customize your settings beforehand, but Identify is a hands-off function unlike the Tagger views. There's no way to verify a match is correct before its info is saved locally. It is highly recommended to **back up your database before running Identify** in case you need to revert any unintended changes. Because of the lack of manual verification, it also does not submit your fingerprints to StashDB during this process. The Scene Tagger is still the only way to do that.

Finally, if you have [edit access]({{ site.baseurl }}/docs/faq_getting-started/stashdb/contributing-to-stashdb/), you can add/update scenes and performers to StashDB by submitting drafts directly from within Stash. See [this section]({{ site.baseurl }}/docs/faq_getting-started/drafts/submit-from-stash/) for more details on how to submit drafts.
