---
title: "Fixing nicenames (when page not found message displayed instead of profile): Procedure"
---

Sometimes it will happen that a user will appear to be set up correctly but instead of their WP profile page you see a &ldquo;page not found error.&rdquo;

This happens when old usernames were not migrated properly from the old system, and it only occurs with users that existed before we relaunched in 2014.

PROCEDURE:

1. get &ldquo;page not found error for username&rdquo; - oops.![|422x231](https://community.namati.org/uploads/default/original/2X/6/6660c5ac78d3cf7622d4623962ac33f2ea9bf636.png)

2. open [my.wpengine.com](https://my.wpengine.com/) and navigate to phpmyadmin for our live site

3. keyword search all tables for username, navigate to the user table row with a hit![|624x37](/uploads/default/original/2X/9/94bca517b08a23e0840f979e4366ed607f23347f.png)

4. click into the &quot;nicename&quot; field and change it to the correct username. click out of the field to save changes.![|551x128](/uploads/default/original/2X/e/ed3fce83ba5849c9065afd94ec9b4d7cf3d73d25.png)

5. refresh page in wordpress to confirm the fix worked - yay.![|536x278](/uploads/default/original/2X/2/27d66a7eb2c3349b81e77b5a0d6e46c0b8bbebad.png)

<small class="documentation-source">Source: [https://community.namati.org/t/fixing-nicenames-when-page-not-found-message-displayed-instead-of-profile-procedure/41159](https://community.namati.org/t/fixing-nicenames-when-page-not-found-message-displayed-instead-of-profile-procedure/41159)</small>
