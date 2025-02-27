Heartland Cyber Range revision history. Descriptions of code updates and patch notes can be found here. The HCR LMS code base is maintained in a separate, private repo.

---

## v0.2.0.022725 ***Pre-release***

This beta pre-release adds a functional support ticketing system, whereby users can submit feedback and create support tickets. A separate support ticketing system is now implemented that will be used to track customer issues. The support form and access to the support ticketing system is available within the LMS by clicking on the support icon in the left-hand nav bar (lower left, headset icon). Additionally, numerous UI improvements and fixes were implemented - among them:

   - The following site pages have been updated to match the current HCR theme:
        - User profile page
        - All "page" resources
        - auth/oauth2/login.php
        - mod/foundry/view.php
        - support/feedback.php
        - report/log/user.php
        - report/performance/index.php
   - The Foundry Appliance resource page was updated to add additional CSS selectors, "Gamespace Resources" was updated to read "Virtual Lab Resources", and all other "Gamespace" nomenclature also changed to "Virtual Lab"
   - The login page layout was adjusted to remove (hide) the local login form (as users will use OpenID to log in, and the local login form being present just confuses users), as well as to rearrange elements, adjust font sizes, etc. to improve the UX. The help '?' icon was adjusted to a round button, and updated the "Powered by" message to read "Powered by the next generation Ora Nexum network.".
   - Added a "Category: " prefix to the category title section at the top of the category browser view, and centered the text.
   - Created separate back-end CSS files for organization and added new CSS updates:
        - Removed box-shadow and border artifacts from login page, from a previous theme.
        - Added drop shadows to the messaging drawer for improved visibility/contrast with the underlying page.
        - Removed the id badge #'s from top level categories in the course browser.
        - Extended the char count on category buttons (for handling overflow, with long names) so more of the category name is readable.
        - Applied a border-radius to the search box.
        - Changed the notifications badges for new messages/notifications from rectangular to rounded.
        - Resolved a problem with the category browser where categories could be expanded (to show subcategories) but could not be collapsed again.
        - Centered and shrank the "mark as done" button and wrapper div to the size of the button (rather than stretching across the whole screen), made background transparent. (Button, when present, will now show as a lone button near the top center).
        - Added a white background with border-radius to the editing section of a user's profile. The additonal contrast helps immensely with visibility/UX
        - Fixed the hover/active/focused CSS For top nav-bar links (mostly visible in admin settings): rounded the edges of the focused/active section, made the hovered tab background transparent (indexing was causing the hovered tab to overwrite the border of the adjacent, selected tab).

---

## v0.1.0.012325 ***Pre-release***

This beta pre-release adds the full LMS code base to the repo. Additionally, a number of UI updates were introduced since the original dev group was removed from developing further code:

   - Approximately 175 CSS updates were made, to bring the UI experience closer to the original mock-ups.
   - The full set of navigation icons were introduced to the left hand navigation bar. Icons for features that are not yet implemented are inactive.
   - The elements on the login form were rearranged to prevent confusion on how to log in.
   - Theme renderer code was updated to correct some issues:
       - Instead of displaying only the top level categories (domains) on the content browser, all categories and sub-categories were showing. This was corrected to only display the top level categories.
       - The preview section would only display a preview for content directly under that specific category. Reworked the code to traverse the category tree and display both sub-categories as well as courses/modules.
   - Moodle Adminer was added to the admin control panels and restricted to the site admin.
   - An 'HCR Adminstrator' role was created, to provide administrative access to appropriate users, without having to provide site admin (super user) level access.

---

## v0.0.0.092024 ***Pre-release***

Code dump from original dev group, containing only custom theme file updates.

---
