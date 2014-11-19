## Pageshot

This is a prototype addon to try ideas around freezing the DOM and sharing the result.  You can view the site (with a link to install the Add-on) at [pageshotpages.appspot.com](https://pageshotpages.appspot.com)

It is a Firefox Add-on, using the [Add-on SDK](https://developer.mozilla.org/en-US/Add-ons/SDK) and a website using Google Appengine.  The addon is in the root, and the website is in `appengine/pageshotpages/`

Much of the interesting work about what you can do with the page after it is frozen will go in `appengine/pageshotpages/js/`.  The addon mostly just freezes the content.

Known issues:

- Iframes don't get frozen.  This is a permission problem with Add-ons.  I guess I have to do something [described here](https://developer.mozilla.org/en-US/Add-ons/SDK/Guides/Content_Scripts/Cross_Domain_Content_Scripts) (though how to do it for all domains is unclear).
- You should be using Firefox Aurora (or Developer Edition), or Firefox Nightly
