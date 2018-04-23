---
title: Activate user account on behalf of a new member
---

When a new user registers for the network, their account is not actually created until they click an activation link they receive by email.

Sometimes we have to activate the account on their behalf because they don&rsquo;t do it on their own.

Here&rsquo;s how to do it:

1. using chrome web browser, log in as admin and go to https://namati.org/wp-admin/admin.php?page=gf_edit_forms&amp;view=settings&amp;subview=gravityformsuserregistration_pending_activations&amp;id=1

2. Review the list of pending activations, and make any obvious fixes to typos in email addresses that might have caused the activation to not happen

3. to activate one of the pending accounts, right click (or cmd-click on mac) on the ACTIVATE link and select &ldquo;open link in incognito window&rdquo;. Then close the incognito window to go back to the list.

4. that&rsquo;s it! You may need to write to the user to let them know but they will now get the welcome PM in their email via discourse. 

WHEN do we need to do this? Oftentimes, users who only register but don&rsquo;t click the link to activate their accounts are stuck without an active account. To decide if we should activate it for them, we&rsquo;ll follow the steps below:

* check in salesforce for the email address.

* if it exists and has a 2+ rating, activate on behalf of the user.

* if it exists but has a typo, fix it and then activate on behalf of the user.

* if it does not exist and it's spam or a test account, just delete it.

* if it does not exist and is not spam, send an email to the address asking for followup, then keep an eye out for a reply. If no reply after a while, delete it.

<small class="documentation-source">Source: [https://community.namati.org/t/activate-user-account-on-behalf-of-a-new-member/41151](https://community.namati.org/t/activate-user-account-on-behalf-of-a-new-member/41151)</small>
