tsu-friends-and-followers
=========================
Author: Armando Lüscher

Version: 1.0

Details
=======
Tsu script to display Friends and Followers of all users on the current page.

Use this script to display the number of Friends and Followers a user has, right next to / under their user name.
Gain control over who has how many Friends and Followers with a quick glance.
Furthermore, it generates links to all users displayed on the "Discover Users" page, to make it easier to check out the profiles.

The details get loaded automatically when the page gets loaded and automatically updates itself when new posts, comments or messages get added.

A link "Load Friends and Followers" gets added to the menu at the top right, to force a reload of all Friends and Followers. This is useful if you just want to update / re-fetch the up-to-date details without having to reload the page.


Installation
============
- Firefox: Install the GreaseMonkey plugin and add the script to the library.
- Chrome: Install the Tampermonkey plugin and add the script to the library.

Alernatively, you can just minify the script and create a bookmark in your browser's toolbar to execute the code on the current page. This will have to be done every time the page is reloaded.

Script can be found here:
- https://github.com/noplanman/tsu-friends-and-followers/raw/master/Tsu_Friends_and_Followers.user.js
- https://greasyfork.org/en/scripts/6108-tsu-friends-and-followers
- https://openuserjs.org/scripts/noplanman/Tsu_Friends_and_Followers

How does it work?
=================
Basically what happens, is that the script searches the page for user links and then loads their user page in the background. From that loaded page, the number of Friends and Followers gets extracted and displayed nicely next to / under the user link.
The details get saved and are reused when the same user name appears multiple times. This makes sure that each user is only loaded once, to save precious time and bandwidth. Using the menu button to freshly load Friends and Followers, clears the saved entries and reloads them all, as you might have guessed.

I will try to keep this script up to date and am very much looking forward to an official API from Tsu to make things quicker and more reliable.


Any Ideas / Feature requests / comments?
========================================
If you have any ideas for me or things you would like to see in this script, just create an "Issue" on the right and let me know!
Any comment is highly appreciated, thanks!


Tested with
===========
- Firefox 33.01
- Chrome 38.0.2125.111


Known issues
============
- Change observer to only call Friends and Followers function when needed. Ignore '.tooltipster-base' due to profile summary popup changes.
- Sometimes the loader wheel stays and doesn't go away.