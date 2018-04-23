---
title: New Member and Organization cleanup in WordPress and Salesforce
---

While most of the action takes place in WordPress and Discourse, we still use Salesforce for the following contact management tasks: 

- Namati contact management (fundraising, mailing list, etc) 
- Managing contacts who apply/register/attend network events (organized into "salesforce campaigns") 
- Inviting contacts to join the network (keep track of invite status using "network invitation" field on contacts view) 
- Triaging inquiries received by email and determining appropriate response, and by whom (is contact a member? mailing list subscriber? have they attended an event or partnered with Namati in the past?) 

For the above to work, we need to perform a few steps for each and every new member who joins the network - on a timely basis! :mantelpiece_clock:  Preferably on the same day or at the latest within a few days.  

<details><summary>Step 1: Review profile in WordPress</summary>

* Log into WordPress as admin and [open the User list](https://namati.org/wp-admin/users.php). Here you can check to see which new members don't have a value for "Salesforce ID" - these are the ones you need to review. 
* Select CTRL (CMD on mac) on your keyboard and click VIEW under member's username to open the member's profile in a new tab. Here you can scan the profile details (name, country, bio, affiliation) to start to get to know the member. 
- If the member has an organization, CTRL/CMD-Click through to see the organization profile in a new tab. 
    - Remember - this is a new member we want to encourage to return and become active in the community, so we want to do our best to help them get started - especially if they have an organization and are a legal empowerment practitioner. 
    - This is also the moment to take care of any edge cases - e.g. spam user to delete, duplicate that needs to be merged, extraneous org profile, etc. 
- Assuming all well and we want to keep this member, move on to step 2. 
</details>
<details><summary>Step 2: Merge contact records in Salesforce</summary>

* In another browser tab, log into [Salesforce](https://login.salesforce.com) and copy/paste the member name into search field at [Salesforce Merge Contacts](https://namati--npe01.na46.visual.force.com/apex/ContactMerge?sfdc.tabName=01ri0000000bQUs). You will usually see two or three results - select them all to merge them.  If there are more than three matching contacts, you will have to do this step twice. 
* press `NEXT`. On the resulting page, select the &ldquo;master record&rdquo; based on which record has the most complete information, then go through each field and make sure the correct info is selected, pay particular attention to the following:
    * correct first name and last name = selected 
    * mailing country and other country = blank 
    * title = blank 
    * contact description = blank
    * add to mailchimp = selected
    * Network member = selected 
    * household = same as master record (otherwise merge may fail) 
    * WP username and WP user ID = selected (and match wordpress) 
    * email address = matches address in wordpress (if there are two, copy one and paste it into an other email field in the next step) 
* once you've gone through these fields, select `merge` button
    * you'll be re-directed to the new (merged) contact record; now we can proceed to step 3.</details>

<details><summary>Step 3: make a few updates to member's contact record in salesforce</summary>

* `contact type` = `practitioner.` 
   - Note: Other staff may also be adding other types to this list so leave those alone.
* if 'Network Invitation' is not blank, change it now to "invited as a result of invitation". 
* Title = blank
* Copy WP username, discourse username, and WP user nicename from WP into SF
* WP user ID is correct and matches wordpress (look in info box on wordpress profile page)
* `date registered` exists and matches wordpress
* `add to mailchimp` box is selected
* copy `WP: Username` to `Discourse Username` and `WP: User "Nicename"` = they should all be the same. 
  - Note: if the username is an acronym of their organization or contains numbers, you want to change it first in WordPress/Discourse, then come back here to continue. [Procedure](https://community.namati.org/t/procedure-change-a-network-members-username-wordpress-and-discourse/1189?u=tobiaseigen)
* copy the `salesforce ID` and then navigate to the user's wordpress profile using the `Open in WordPress (Admin Edit)` link, opening it in a new tab. paste the salesforce ID into the wordpress field `Salesforce ID`
  - while you're in wordpress, check and make any improvements to the member's profile. Check all fields but especially the name (no all caps) and bio (fix typos).  
* make sure to press `save` at the top of the SF page when done, and `update user` at the bottom of the WP page when done</details>

<details><summary>Step 4: Additional steps if new member has indicated organziational affiliation</summary>

* if member's affiliation in WordPress is clearly incorrect (this happens quite often) you can remove it, usually without letting the member know. 
  - reasons: bio describes different affiliation than that chosen, country/continent is totally different, organization profile is an extension of the member profile
* if member's affiliation to an existing organization is clearly legitimate, go ahead and change `status` to `active affiliation` in WordPress -- if you are unsure, change it to `pending`
  - reasons: they added it themselves, email address matches, listed on official website, etc
* While still in the individual's contact record in Salesforce
   * organization name = search for and add organization name, if one exists in wordpress or leave it as it is (defaults to be same as name). Save contact. 
* click into the individual's organization (under `Organization Name`)
   * Open the organization in WordPress in admin edit mode
* Sometimes the organization profile will not exist in Salesforce for mysterious reasons. When this happens, create it manually. 
    - copy the organization name from wordpress to clipboard
    - in the salesforce contact, search for the organization and paste in the name of the organization. select "NEW" to create it - and add city and country at the same time. 
    - save the contact, then click on the organization name to edit it. 
    - fill in these fields and save changes.  
         - network roganization directory name
         - wordpress org id
         - directory URL 
* Copy the Organization ID (long) from Salesforce into the Salesforce ID field in the organization&rsquo;s wordpress page
</details>

There are also some periodic bulk cleanup tasks - to fix various contact fields and to make sure the data is reasonably up to date in both places. Procedures TBD in a new wiki topic.

<small class="documentation-source">Source: [https://community.namati.org/t/new-member-and-organization-cleanup-in-wordpress-and-salesforce/42057](https://community.namati.org/t/new-member-and-organization-cleanup-in-wordpress-and-salesforce/42057)</small>
