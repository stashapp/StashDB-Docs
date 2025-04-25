---
layout: default
title: Accessing StashDB
nav_order: 1
has_toc: true
parent: 'StashDB'
grand_parent: FAQ / Getting Started
---

# Accessing StashDB
{: .no_toc }

{: .important }
**Details on joining StashDB and connecting it to Stash.**

---

<details open markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Creating an Account
You will need to register an account on StashDB.org before you can view or access any of its data. The process should be fairly straightforward, but here's a step-by-step guide just in case.

New accounts start with READ access only. If you'd like to add or edit any data on StashDB.org, you will need to [ask for EDIT access]({{ site.baseurl }}/docs/faq_getting-started/stashdb/contributing-to-stashdb/) after creating your account.

1. **Go to [https://stashdb.org/register](https://stashdb.org/register){:target="_blank"}**
1. **Enter a valid email address**
    - This email address will only be visible to StashDB admins. It will not be used as your username.
    - Do not forget it, you will need it if you ever need to reset your password. An admin may also ask you to provide this address if you need their help with your account.
1. **Enter an active invite key**
    - Copy and paste this entire code into the registration form: <br> {% include invite-code.txt %} <br> It has a limited number of uses so it will be replaced periodically.
    - A different invite code is available in [this topic](https://discourse.stashapp.cc/t/how-to-register-on-stashdb/402){:target="_blank"} on [Discourse](https://discourse.stashapp.cc/signup){:target="_blank"}, in case the code above has expired.
    - If any of these codes have expired, please ask politely for it to be refreshed by contacting **@AdultSun** on Discourse or Discord. A few other elevated users can also generate invite codes if necessary.
1. **Check for an email from StashDB and click the activation link**
    - Please wait a few minutes for the email to arrive. If you still don't see it, try refreshing your inbox or checking your spam/junk folder.
    - Your activation link is only good for about 2 hours. You'll have to start over if it expires.
    - The link will direct you to a webpage to *choose your username and password for the first time*. This is not a generic login page even though it may look like one at first glance. This has confused others before, so just keep going.
1. **Choose your username**
    - Do *not* enter your email address as your username here.
    - Avoid using special characters like `#` or `/` in your username. A bug in Stash-Box may break the link to your profile page.
    - If you forget your username after linking your account to Stash (see the next section of this article), you can look it up yourself by clicking the "Test Credentials" button under Settings -> Metadata Providers -> Stash-box Endpoints.
    - Admins are able to change or lookup your username upon request. Contact an admin (preferably **@AdultSun** on Discourse or Discord) and provide your email address in a DM to verify your account.
    - If you plan on requesting edit access, we recommend your username in StashDB matches your display name in Discourse and Discord. See the [Contributing to StashDB]({{ site.baseurl }}/docs/faq_getting-started/stashdb/contributing-to-stashdb/) page for further details.
1. **Choose your password**
    - Must be at least 8 characters long while avoiding "common" passwords.
    - Passwords cannot be seen or reset by an admin. You will need to click the "Forgot Password" link on the login page to reset it yourself.
1. **Click the "Create Account" button**
1. **Re-enter your new username and password to log in**
    - You will always need to use your *username* to log in, your email address will not work here.

## Connecting to Stash
In order to pull StashDB's scene, performer, and studio data directly into your local Stash database, you will need to connect your StashDB account to your local Stash installation. This will also allow you to use [generated fingerprints/hashes]({{ site.baseurl }}/docs/faq_getting-started/stashdb/whats-a-phash/) to match your local videos with their entries on StashDB. Our [Guide to Scraping](https://docs.stashapp.cc/beginner-guides/guide-to-scraping/){:target="_blank"} will walk you through how to do all of that after you've connected StashDB to your Stash.

The process below can also be used to link other Stash-Box accounts to your Stash. You'll just need to swap out StashDB's info with the relevant details specific to the Stash-Box you'd like to connect. Those details are listed for several available Stash-Boxes in the [Accessing Stash-Boxes]({{ site.baseurl }}/docs/faq_getting-started/stashdb/accessing-stash-boxes/) page.

1. **Find your unique API key for StashDB**
    1. Log into [StashDB.org](https://stashdb.org/){:target="_blank"}
    1. Click on your username at the top, next to the generic user icon
    1. Copy the entire API key
1. **Find your saved Stash-Boxes in Stash**
    1. Go to the "Settings" page in Stash <br> *(Located at [http://localhost:9999/settings](http://localhost:9999/settings){:target="_blank"} by default)*
    1. Click "Metadata Providers" on the left side
    1. Find "Stash-box Endpoints" at the top
1. **Add StashDB to your saved Stash-Boxes**
    1. Click the "Add" button
    1. Paste your API key
    1. Enter `StashDB.org` as the "Name" <br> *(Or use whatever else you want StashDB to be listed as, it doesn't need to be exactly the same.)*
    1. Enter `https://stashdb.org/graphql` as the endpoint
    1. Click the "Confirm" button
