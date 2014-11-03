#Tsu Friends and Followers

Author: Armando Lüscher

Version: 1.1 ([changelog](https://github.com/noplanman/tsu-friends-and-followers/blob/master/CHANGELOG.md))

Short Link for sharing: https://j.mp/tsu-friends-and-followers

##Details

Tsu script to display Friends and Followers of all users on the current page.

Use this script to display the number of Friends and Followers a user has, right next to / under their user name.
Gain control over who has how many Friends and Followers with a quick glance.
Furthermore, it generates links to all users displayed on the "Discover Users" page, to make it easier to check out the profiles.

The details get loaded automatically when the page gets loaded and automatically updates itself when new posts, comments or messages get added.

A link "Load Friends and Followers" gets added to the menu at the top right, to force a reload of all Friends and Followers. This is useful if you just want to update / re-fetch the up-to-date details without having to reload the page.


##Installation

###With Plugin (recommended)

1. Which browser?
  - Firefox: Install the [GreaseMonkey](https://addons.mozilla.org/en-US/firefox/addon/greasemonkey/) plugin.
  - Chrome: Install the [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo?hl=en) plugin.
  - Safari (untested): Install the [NinjaKit](http://www.pimpmysafari.com/items/NinjaKit-GreaseKit-for-Safari/) extension.

2. Friends and Followers script can be found here (just choose any one)
  - https://github.com/noplanman/tsu-friends-and-followers/raw/master/Tsu_Friends_and_Followers.user.js
  - https://greasyfork.org/en/scripts/6108-tsu-friends-and-followers
  - https://openuserjs.org/scripts/noplanman/Tsu_Friends_and_Followers

###With Bookmarklet (to give it a try)

Alternatively, you can just create a [bookmarklet](https://en.wikipedia.org/wiki/Bookmarklet) in your browser's bookmarks toolbar to execute the script on the current Tsu page you're on.

1. Right click you bookmarks toolbar and choose "New Bookmark" or open your bookmarks panel and choose "New Bookmark".
2. Give it a name (e.g. Display Tsu Friends and Followers) and in the location / destination field add the whole line you can find [here](https://github.com/noplanman/tsu-friends-and-followers/raw/master/Tsu_Friends_and_Followers_Bookmarklet.txt).
3. Visit Tsu and click on the newly created bookmarklet.
4. Mind blown!

*Note: With this method, you will have to click the bookmark / run the bookmarklet every time the page is reloaded. Therefore, the plugin variant is highly recommended.*


##How does it work?

Basically what happens, is that the script searches the page for user links and then loads their user page in the background. From that loaded page, the number of Friends and Followers gets extracted and displayed nicely next to / under the user link.
The details get saved and are reused when the same user name appears multiple times. This makes sure that each user is only loaded once, to save precious time and bandwidth. Using the menu button to freshly load Friends and Followers, clears the saved entries and reloads them all, as you might have guessed.

I will try to keep this script up to date and am very much looking forward to an official API from Tsu to make things quicker and more reliable.


##Any Ideas / Feature requests / Comments?

If you have any ideas for me or things you would like to see in this script, just create a [New Issue](https://github.com/noplanman/tsu-friends-and-followers/issues/new) and let me know!
Any comment is highly appreciated, thanks!


##Tested with

- Firefox 33.01
- Chrome 38.0.2125.111


##Known issues
- Change observer to only call Friends and Followers function when needed. Ignore '.tooltipster-base' due to profile summary popup changes.
- Sometimes the loader wheel stays and doesn't go away.
