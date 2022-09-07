---
layout: default
title: "Getting Started: StashDB"
nav_order: 2
---

# **Getting Started: StashDB**
{: .no_toc }
The following sections are general advice and explanations for potentially confusing aspects in our database. Because they don't represent explicit decisions concerning database management or curation, they do not require formal approval. Additional **Getting Started** sections specific to [Performers]({{ site.baseurl }}/docs/performers/getting-started-performers/), [Scenes]({{ site.baseurl }}/docs/scenes/getting-started-scenes/), [Studios]({{ site.baseurl }}/docs/studios/getting-started-studios/), and [Tags]({{ site.baseurl }}/docs/tags/getting-started-tags/) can also be found under their respective categories in the navigation tree to the left. The sections below cover broader subjects that are not exclusive to one of those four categories.

<details open markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

***

### What is StashDB?
- **Our shared database of scene, performer, and studio metadata. Does not host video files or unofficial download links.**

StashDB is our shared public instance of the Stash-Box software. It hosts information about a wide variety of scenes, studios, and performers that can be easily pulled into your own installation of Stash. It does not host any video files or link to any unofficial downloads. Very few users will have reason to host or install a Stash-Box instance themselves, so if you're confused by the terminology just focus on [linking StashDB to your local installation of Stash](#accessing-stashdb). Detailed instructions for connecting to StashDB can be found in the pinned messages of our **#stashdb-invites** channel on [Discord](#joining-our-discord).

### What Makes StashDB Better?
- **Full integration with Stash and improved scene matching using various fingerprints (PHashes).**

StashDB is not the only source of much of its metadata. When filling out information in Stash, you will likely use multiple sources to cover various parts of your collection. Stash has a helpful [repository of scrapers](https://github.com/stashapp/CommunityScrapers) to assist with that. Each source will have its own strengths and weaknesses, just like StashDB. However, the main advantages of using StashDB over similar databases are:
1. **Full continuing integration with Stash.** Stash, Stash-Box, and StashDB are all part of the same shared project. They all enjoy the benefits of parallel development, always keeping each other in mind when creating or updating new features. Updating info in Stash from StashDB should be easier and more versatile than using other sources, just as updating StashDB from within Stash should become more convenient as well.
2. **The ability to match your files with scene entries on StashDB using hashes/fingerprints alone.** With the inclusion of [perceptual hashes](#whats-a-phash), even files of differing resolutions, encodes, or download sources will often be similar enough to still match with StashDB. In other words, your files and their hashes don't have to be exact matches with the fingerprints on StashDB. Stash will be able to find matches as long as your video _looks just similar enough_ to somebody else's fingerprint submission. This level of fuzzy matching makes our system much more reliable, flexible, and versatile than alternative approaches.

### Joining Our Discord
- **Necessary for accessing StashDB, click link for details.**

The Stash Discord server is your best bet for finding help and resources relating to Stash, Stash-Box, and StashDB. You will need to have a Discord account and join our server in order to [access StashDB](#accessing-stashdb). You could create a temporary throwaway account on Discord for this purpose if you'd like. However, if you would like to [contribute more than just hashes to StashDB](#contributing-to-stashdb), you will also be expected to be reachable on Discord. If you've already joined, the link is in the sidebar to the left.

[Click here to join our Discord server.](https://discord.gg/2TsNFKt)

### Accessing StashDB
- **Must create an account, details found on Discord.**

You will need to create a StashDB account to access it from within Stash. Instructions for creating an account and connecting it to Stash can only be found in [our Discord server](#joining-our-discord) at this time. Look for the pinned messages in the **#stashdb-invites** channel for detailed instructions.

### Using StashDB
- **Tagger Views are recommended for pulling info from StashDB, Identify task is faster but less accurate.**

The recommended method for pulling information from StashDB into your local Stash is through the Tagger view. The Tagger can be found on both the Scenes page and the Performers page by clicking on the double-label icon on the far right end of the toolbar near the top of the webpage. With the [Scene Tagger](https://github.com/stashapp/stash/blob/develop/ui/v2.5/src/docs/en/Tagger.md), you can match your scenes with StashDB entries by keyword or fingerprint, save that information to your scene including a link to StashDB called the StashID, and submit your fingerprints back to StashDB to help other users match their own scenes. Be sure to check out the "Scrape All" button (limited to one page at a time), the green checkmarks to customize which fields to overwrite, and the gear icon for additional settings. If you've already found your scene's entry on StashDB, you can paste the [StashID](#whats-a-stashid) directly into the "Query" field to ensure an accurate match. See this [same link embedded above](https://github.com/stashapp/stash/blob/develop/ui/v2.5/src/docs/en/Tagger.md) for more details from Stash's in-app manual.

The Performer Tagger works similarly. Don't miss the "Batch Add Performers" and "Batch Update Performers" buttons on the top right, with a "Show Configuration" link on the opposite side. You can still paste the [StashID](#whats-a-stashid) directly into the search field if you've found the correct performer entry on StashDB already. Individual fields can be turned on and off for each scrape as well.

The [Identify](https://github.com/stashapp/stash/blob/develop/ui/v2.5/src/docs/en/Identify.md) task can also pull scene info from StashDB. You can customize your settings beforehand, but this is a hands-off automated function unlike the Tagger views. There's no way to verify a match is correct before its info is saved locally. Because of this lack of manual verification, it does not submit your fingerprints to StashDB during this process. The Scene Tagger is still the only way to do this.

Finally, if you have [edit access](#contributing-to-stashdb), you can add scenes and performers to StashDB by submitting drafts directly from within Stash. From within a scene's details page, click on the three vertical dots in the top right of the details pane and select the "Submit to Stash-Box" option. Clicking the "Submit" button in the resulting dialog box will save a draft to create that scene/performer on StashDB using the information you have saved locally. From the [Drafts](https://stashdb.org/drafts) page, you can make any necessary changes, leave an [edit comment](#edit-comments), and finally submit your draft to be [approved](#voting-on-stashdb) just like any other edit.

### What's a PHash?
- **Perceptual hashes are generated from what a video looks like, allowing for more reliable scene matching with StashDB.**

[Perceptual hashes](https://hackerfactor.com/blog/index.php%3F/archives/432-Looks-Like-It.html) (PHashes) are one of the main reasons why we [recommend using StashDB](#what-makes-stashdb-better) with Stash. PHashes are used to match your video files with scene entries on StashDB. Even files of differing resolutions, encodes, or download sources will often be similar enough to still match with StashDB. In other words, your files and their hashes don't have to be exact matches with the fingerprints on StashDB. Stash will be able to find matches as long as your video _looks just similar enough_ to somebody else's fingerprint submission. This level of fuzzy matching makes our system much more reliable, flexible, and versatile than alternative approaches. PHashes can also be used in Stash to detect duplicate files in your library, using the "Scene Duplicate Checker" in the "Tools" tab of the Settings page.

PHashes are not generated in Stash by default, so you will need to create them yourself. They may be generated during a Scan by activating the switch next to "Generate perceptual hashes" or through the Generate task (in the "Tasks" tab of the Settings page or the "Generate..." option with individual scenes selected) next to "Perceptual hashes (for deduplication)". These may be submitted to existing scenes on StashDB along with other fingerprints using the [Scene Tagger](#using-stashdb) and will be included automatically when [submitting new scenes via draft](#using-stashdb).

### What's a StashID?
- **Unique ID for entries in StashDB, found at the end of URLs and saved to Stash after a match.**

A StashID is the unique identifier for an entry on StashDB. It can be found in the URL of a scene/performer/studio entry as the string of seemingly random numbers and letters at the end. StashIDs can be saved to your own scenes, performers, and studios in Stash when using the [Tagger view or Identify function](#using-stashdb) as well as a Stash-Box scraper. This links your local entries in Stash to their match on StashDB for future reference and scrapes.

As there is no Studio Tagger or studio scraper support, the Scene Tagger view is currently the only way to attach a StashID to a locally saved studio. The Tagger will give you several options to choose from when it doesn't find a studio's StashID saved anywhere locally. From left to right, you can create a new studio with the suggested name and StashID (no other details are saved at this time), skip the studio field entirely, or attach the StashID to a studio you've already created. This last option will be selected automatically if a studio's primary name or an alias exactly match the name of the suggested studio on StashDB. Be sure to click the floppy disk icon to save your selected action, creating the new studio or attaching the StashID.

### Contributing to StashDB
- **Submitting fingerprints is possible with every account, but any other edit/submission requires permissions granted through Discord.**

Every StashDB account is able to submit fingerprints/hashes from within the Scene Tagger view of Stash. This does not require any additional permissions. However, if you would like to add or edit performers, scenes, studios, or tags, you will need to be granted additional privileges. Requesting edit access is not difficult. Detailed instructions can be found pinned to the **#stashdb-invites** channel on [Discord](#joining-our-discord). Please note that you will be expected to be reachable on Discord if you become an active contributor on StashDB. This is because there is no messaging or notification system from within StashDB at this time. If we cannot reach you over Discord, your edit rights may be revoked by an admin after repeated violations of our guidelines.

### Bulk Edits
- **Big projects that require a large number of edits should be pitched on Discord first for approval.**

Any projects that would affect a large amount of data on StashDB and/or require a high volume of individual edits will need to be approved on Discord first by dropping a question in the **#stashdb-general** channel. If it's in line with the guidelines already established on this Wiki, than a simple "heads up" before starting may be all that is needed from you. More drastic changes may require formal approval as a [guideline proposal](#guideline-proposals) in the **#stashdb-guidelines** channel on Discord. Projects that would add more than a few dozen edits into the queue at a time may need to be broken up into smaller chunks. All of these points apply to both manual submissions and automated submissions.

### Voting on StashDB
- **Different voting thresholds apply to destructive vs. non-destructive edits. Voting rights granted automatically after 10 approved submissions.**

All edit submissions to StashDB will be subject to approval by the votes of other contributors. Voting rights will be granted automatically once you have 10 submissions approved.

Edits considered non-destructive may be approved immediately if they receive three unanimous YES votes. They may also be rejected immediately with three unanimous NO votes. Destructive edits (Merge and Destroy requests, mostly) and non-unanimous vote totals will require a waiting period to pass before it is rejected or approved. This may be 3 days or 7 days, depending on the current vote total. Net totals of 0 votes will still be approved at the end of the waiting period for non-destructive edits but will be rejected for destructive edits. For more details on a particular edit, hovering your cursor over "Voting closes in X days" in the top right corner will show you if it will be rejected or approved with the current vote total as well as the exact day and time the voting period will end.

The ABSTAIN option is only used if you would like to remove your YES or NO vote rather than changing it. The "Save" button will not appear when ABSTAIN is selected unless you have previously saved a YES or NO vote on that edit.

### Asking for Votes
- **Asking on Discord is discouraged unless the edit needs to be approved before additional edits can be submitted.**

Typically, asking on Discord for votes to approve your own edit is seen as impolite. Many see it as similar to jumping to the front of the line instead of waiting your turn. There are exceptions to this though. Often edits act as "blockers" to other edits. Maybe someone has a scene they want to add to StashDB, but they need a performer or studio to be approved first before they can be attached to the scene submission. The performer/studio submission is considered a "blocker" to the scene submission, so it would be appropriate to ask in the **#stashdb-general** channel on [Discord](#joining-our-discord) to expedite its approval. In cases like these, longer approval times actually do inconvenience the contributor where waiting on typical edits would not.

### Unconfirmed Guidelines
- **Still expected to be followed but subject to change pending formal approval.**

Early on, many of this Wiki's sections will have this message at the bottom:

_Unconfirmed guideline, subject to change pending formal approval._

All this means is that the language has not been formally approved by the community in our **#stashdb-guidelines** channel on [Discord](#joining-our-discord) yet. Contributors are still expected to follow these unconfirmed guidelines, but should know that they are subject to change in the near future.

### Guideline Proposals
- **Changes to guidelines require formal approval, so ask about it on Discord first.**

If you would like to make a change or addition to the guidelines in this Wiki, please ask about your idea in our **#ministry-of-truth** channel on [Discord](#joining-our-discord) first. If your suggestion gains traction there, a formal proposal will need to be approved by the community in the **#stashdb-guidelines** channel. Only users with elevated Discord roles will be able to post proposals there.

### Edit Comments
- **Say what you're doing, why you're doing it, and what your sources are.**

Regardless of what kind of edit you're submitting, always include in the comment field what you are doing and why. Bigger or more drastic changes will likely require longer comments, but simple changes likely won't need much. Also please remember to note what you are using as the source of your edit when appropriate. These notes will be helpful when considering further edits in addition to justifying your actions now to those who will be voting on it.

### Low Effort Submissions
- **Submissions may be rejected as "low effort" if it will take more time/effort to fix than it would've taken the OP to do correctly in the first place.**

Submissions of any kind may be rejected if voters deem them to be "low effort" even if it doesn't technically violate any other guidelines and all of its information is correct. "Low effort" submissions appear rushed and often leave out information that is obvious or easily found. The reasoning behind rejection is that "low effort" submissions will take the same amount of time and effort for others to fix (if not more) as it would have taken the original contributor to make a complete submission in the first place. It will also often be faster and easier for the original contributor to update or cancel/redo their own submission than for somebody else to do it for them.

"Low effort" submissions should not be confused with small edits, which are of course welcome on StashDB. If you fear that your edit may appear incomplete to others and could be at risk of downvotes as a "low effort" submission, make sure you explain why your edit may look that way (performer not listed anywhere, couldn't find any details/photos for a performer, waiting for another edit to be approved before you can add something, etc.) Voters won't be inclined to downvote if you acknowledge and explain a sparse edit. Also, please see our related policy on [missing scene performers]({{ site.baseurl }}/docs/scenes/scene-performers/#missing-scene-performers).

### Backlog Spreadsheet
- **Anything that can't be fixed from within StashDB yet should be logged here, including incorrect fingerprints.**

Not everything can be fixed directly from StashDB's UI. For these exceptions, we have a spreadsheet hosted on Google Sheets to log corrections until they can be handled at a later date. There are several pages in the backlog, so make sure you find the correct one. Its most common use right now is to log incorrect fingerprints.

[Our backlog spreadsheet can be found here.](https://docs.google.com/spreadsheets/u/0/d/1eiOC-wbqbaK8Zp32hjF8YmaKql_aH-yeGLmvHP1oBKQ/edit)

### AdBlockers
- **Turn them off on StashDB, otherwise some images will appear "broken".**

Be sure to disable you browser's ad-blocker for StashDB's domain, or add the domain to the allow/white list. StashDB does not host ads of any kind, but some image URLs will get false-flagged as advertisements and will fail to load. These images will appear to be broken on the webpage.