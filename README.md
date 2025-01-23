Heartland Cyber Range LMS code base. The HCR LMS is based off of Moodle and follows the recommended coding practices for that platform.

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
