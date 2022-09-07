---
layout: default
title: "Getting Started: Tags"
nav_order: 1
parent: Tags
---

# **Getting Started: Tags**
{: .no_toc }
The following sections are general advice and explanations for potentially confusing aspects in our database for tags. Because they don't represent explicit decisions concerning database management or curation, they do not require [formal approval]({{ site.baseurl }}/docs/getting-started-stashdb/#guideline-proposals).

***

<details open markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

***

### Picking Tags for a Scene
- **Start small with "important" tags first, expand as you get more familiar with StashDB's list.**

The list of tags on StashDB is long. You don't have to be aware of all of them. You don't have to add every tag that possibly fits. Think of tags as an additional way to describe a scene and focus on adding tags you think are important to describing the scene in front of you. That may require relatively few tags or it could require a lot. You may as well start small and slowly expand from there as you become more familiar with the tags available on StashDB. If you have any questions about how to use a particular tag, first read its description carefully. [Previous edit comments](#tag-edit-comments) may give you more information as well. Otherwise, feel free to ask in the **#ministry-of-truth** channel on [Discord]({{ site.baseurl }}/docs/getting-started-stashdb/#joining-our-discord). Also, please explain in your own edit comment [where your tags are coming from]({{ site.baseurl }}/docs/tags/assigning-tags/#priority-sources-for-tags), if they're simply scraped or if you've added/removed some yourself.

### Tag Edit Comments
- **Say what you're doing, why you're doing it, and what your sources are.**

Regardless of what kind of edit you're submitting, always include in the comment field what you are doing and why. Bigger or more drastic changes will likely require longer comments, but simple changes likely won't need much. Also please remember to note what you are using as the [source of your edit]({{ site.baseurl }}/docs/tags/assigning-tags/#priority-sources-for-tags) when appropriate. These notes will be helpful when considering further edits on the tag later in addition to justifying your actions now to those who will be voting on it.

### Read Tag Edit Histories
- **Comments in the "Edits" tab will often explain why a tag is organized a certain way, so check it first before making an edit.**

If you're wondering why a tag is named/defined/organized a certain way, often the answer is in its edit history. In a tag's detail page, click on the "Edits" tab underneath its list of aliases. The comments on these edit submissions often explain the reasoning behind them, sometimes at great length. If you feel like a tag needs to be changed or merged in some way, please look through these edit comments first. They may show you that an idea has already been considered and explain why it hasn't been implemented.

### Check Tag Usage
- **Look at the scenes underneath a tag to get an idea of its current usage before submitting a destructive edit or description change.**

Before submitting an edit to a tag, always look through the scenes underneath it first. Most tags are defined to [match their current usage](#scraped-vs-manual-tags), so you will need to have a good idea of how it's currently used before you can make an informed decision about how it should be handled. If you're trying to write a new definition for a tag that's missing one, you may find that its scenes are using that tag differently than what you assumed. A tag's current usage, the consistency of its usage, the source of its scenes, and its total number of scene entries will all factor into decisions regarding possible edits.

### Scraped vs. Manual Tags
- **Most tags attached to scenes were scraped from studio sources, not manually added by editors.**

Currently, most tags attached to scenes are scraped from the original studio or some other official source, not manually added from the editors of StashDB. Our current methods of manually adding/removing a scene's tags individually isn't too bad on a small scale, but they are far too tedious and time-consuming to be worth using for large shifts in our tag organization in most cases. This means that most of StashDB's tag list leans on scraped tags in their organization and usage, rather than attempting to enforce major deviations from those sources. This may explain inaccuracies, inconsistencies, or other peculiarities of a particular tag. [Reading through the edit comments](#read-tag-edit-histories) may explain in further detail.

### Sorted vs. Unsorted Tags
- **Tags without categories and/or descriptions are considered "unsorted" and should generally be avoided when manually adding tags to scenes.**

If a tag doesn't have a category or description, then it is likely still unsorted. It will usually have a sparse or non-existent edit history as well. This means it's exact usage hasn't been determined yet, no potential merge targets have been found, and no decision has been made on if it's even worth keeping. It's usually preferable to avoid unsorted tags when manually adding them to a scene yourself. If you're just adding scraped tags though, don't worry if they're currently sorted or unsorted. More scraped sources for an unsorted tag could help us decide what to do with it in the future. Finally, if you want to find a quick list of sorted tags, lean on the [Tag Categories page of StashDB](https://stashdb.org/categories). Every tag with a category assigned will be organized to some extent already.

### Merging and Destroying Tags
- **Unsorted tags that do not have a unique and helpful meaning are candidates for merging/deleting.**

Great care must be taken when merging or deleting tags. When tags are merged or destroyed, it is not easily reversed. Currently, the goal when handling unsorted tags is consolidation. We are aiming to merge all closely related tags together while deleting any that are considered extraneous. The purpose is to create a curated set of tags that are as helpful and as consistent as possible, spanning every studio on StashDB. Just like with other parts of the database, merging is always preferred over deleting. Candidates for a merge/deletion could be tags that seem too vague, too specific, or otherwise irrelevant. These are of course subjective calls, but the rule of thumb should be, "Does this tag have a unique and helpful meaning?" If the answer is "yes", then keep it. If it's "no", then merging/deleting may be the best option. However, we are still trying to be conservative in our approach. Reverting changes can be tricky, so it's better to err on the side of keeping a tag if there's any doubt. Merges should also aim for a resulting tag that is consistent in its meaning. If the inclusion of a tag would result in less consistency of meaning, then it may be best to leave it separate for now. Finally, please remember to include any merged tag names [as aliases](#adding-tag-aliases). This can be done in your merge submission.

### Tag Merge Targets
- **Click "Merge" on the page of the tag you want to keep, then select any tags that should be removed and merged.**

If you click the big blue "Merge" button at the top of a tag's details page, that tag becomes the target of your merge request. In other words, any additional tags selected in the edit request form will be absorbed into that initial tag. Always merge into the tag you intend to keep. Often it will be the only "sorted" tag in your merge with a category and/or definition assigned to it. If you are merging previously "unsorted" tags, your preferred merge target is usually the most frequently used variation (meaning, it has the most scenes attached). Also please note roughly how many scene entries a tag has in your [edit comment](#tag-edit-comments) before merging. There is no easy way to find these numbers after a merge and they are often taken in consideration when choosing [primary names](#changing-a-tags-primary-name). If you would prefer to change the primary name of the tag as well, it is best to save that for a separate edit after the merge is approved.

### Destroying Tags
- **Rarely appropriate, usually there's a potential merge that would be preferred.**

Great care must be taken when deleting tags. When tags are destroyed, it is not easily reversed. Even if a tag seems irrelevant or useless, be sure to use the [search bar](https://stashdb.org/tags) to look for similar tags first. If you find a lot of similar tags or if those tags represent a large number of scenes, then it may be better to merge than to delete. Merging is always preferred over deleting, and [many of the same considerations apply](#merging-and-destroying-tags). Easy candidates for deletion include performer/director names, but make sure these are also saved in the proper fields of all the scenes themselves before submitting your destroy request. Sometimes series titles are used as tags. These can also be easy deletions, but it can sometimes be better to merge it into a similar tag. In these situations, the series title probably doesn't need to be added as an alias.

### Adding Tag Aliases
- **Make sure there aren't any other tags that would be a better fit for an alias, or that another tag isn't using it already.**

Tag aliases on StashDB have limited usefulness at the moment. They do not have the same functionality as Stash's tag aliases. However, we are still trying to use them in anticipation of future updates to both Stash and Stash-Box. Aliases can be used as alternative primary names, reflections of previously merged tags, terms used by a studio not covered by current aliases, alternate spellings, common misspellings, etc. The only limit for tag aliases other than basic relevancy is the following: Are there other tags using this term as its primary name? Are there other tags using this term as an alias? Are there any tags where this term would better fit as an alias? Would this alias be better suited as its own tag?

### Changing a Tag's Primary Name
- **Prioritize brevity, clarity, familiarity, and consistency.**

Since users can rename a tag to anything they'd like from within Stash, a tag's primary name isn't too important. Many will come down to purely subjective personal preference. Because of this, we don't have to worry about Stash too much when (re)naming tags. The main consideration when picking a primary name is how it will be displayed and organized on StashDB itself. Specifically, we want to find a balance between brevity, clarity, and familiarity, as well as its consistency with the naming of other tags. If you feel like a different name would be preferable for a particular tag, be sure to [check its edit history](#read-tag-edit-histories) first to see if it's been considered before or why it's using the current primary name.

### Assigning Tag Categories
- **If the tag you're editing doesn't have a category yet, add one yourself even if you have to guess to mark it as "sorted".**

If the tag you're editing doesn't have a category yet, try to assign one in the same edit. This shows that somebody has handled a tag, [marking it as "sorted"](#sorted-vs-unsorted-tags) to some extent. Categories are easy to correct afterwards, so don't worry about guessing. Also feel free to ask in the **#ministry-of-truth** channel on [Discord]({{ site.baseurl }}/docs/getting-started-stashdb/#joining-our-discord) for clarification.
