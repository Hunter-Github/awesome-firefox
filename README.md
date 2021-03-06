## NOTE: This list is now deprecated and unmaintained since Mozilla has officially turned evil

Hilariously, incompetently evil at that.

* LOOKING GLASS - the tombstone for Mozilla https://news.ycombinator.com/item?id=15931730
* Installing addons covertly - the beginning https://news.ycombinator.com/item?id=15648179
* http://technewslog.com/mozilla-plans-to-collect-anonymous-firefox-browsing-data/
* https://news.ycombinator.com/item?id=15421708
* Mozilla is covertly feeding customer data to Google Analytics. https://github.com/gorhill/uBlock/issues/2784
* Mozilla has systematic deficiencies in vulnerability handling and responsible disclosure
  * https://lwn.net/Articles/656683
  * https://news.ycombinator.com/item?id=12754199
  * https://github.com/mozilla/addons-linter/issues/1000#issuecomment-255089138

# awesome-firefox
A curated list of resources for and about [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/products/) - a [bloated](http://blog.ffextensionguru.com/2015/06/20/mozilla-making-firefox-bloated/) but versatile popular modern browser with nice user interface. Unfortunately, after Firefox 42 Mozilla has instituted unwelcome changes in how addons work entering the already familiar territory of "walled gardens". Please see the [forks](#firefox-clonesforks) chapter to review your alternatives.

## Hardening your Firefox

PSA: Mozilla is covertly feeding customer data to Google Analytics. https://github.com/gorhill/uBlock/issues/2784

**Important security warning** - Mozilla has systematic deficiencies in vulnerability handling and responsible disclosure.
See: https://lwn.net/Articles/656683 https://news.ycombinator.com/item?id=12754199 https://github.com/mozilla/addons-linter/issues/1000#issuecomment-255089138

 * [Changing the configuration](https://github.com/pyllyukko/user.js) - a checklist of things to do with `about:config` to reduce information leaking to Mozilla, Google and other corporate mastodons.
 * [Firefox vulnerabilities](https://web.nvd.nist.gov/view/vuln/search-results?query=firefox&search_type=all&cves=on) - an up-to-date list of vulnerabilities from US NIST (the official Mozilla list is [here](https://www.mozilla.org/en-US/security/known-vulnerabilities/firefox/)).
 * [Certificate Patrol](https://addons.mozilla.org/en-US/firefox/addon/certificate-patrol/) - an extension to watch out for [Man-In-the-Middle](https://en.wikipedia.org/wiki/Man-in-the-middle_attack) (MITM) certificate attacks.
 * [NoScript](https://noscript.net/) - an extension to keep JavaScript activity at a minimum, and protect from cross-site scripting.
  * _Privacy tip_: put `127.0.0.1 secure.informaction.com` into your `hosts` file (NoScript dials home at startup).
 * Adblockers:
  * [uBlock Origin](https://github.com/gorhill/uBlock) - a lighter-weight adblocker. All custom rules from AdBlock Edge can be imported through the clipboard. Has dynamic filters. 
  * <del>[AdBlock Edge](https://bitbucket.org/adstomper/adblockedge/downloads/) - adblocker with a slightly different interface</del> (**discontinued in June 2015**).
  * [uMatrix](https://github.com/gorhill/uMatrix) - request blocker for advanced fine-grained filtering (blocks cookies, iframes, other types of content). Positively awesome, takes no time to learn.  
  * Please note that using ready-made third-party block lists may open up your computer for surreptitiously whitelisted requests - _caveat emptor_!
 * [HTTPS Everywhere](https://www.eff.org/https-everywhere) - an extension to enforce encrypted protected connections no matter what.
 * [GreaseMonkey](https://github.com/greasemonkey/greasemonkey) - a versatile extension to rewrite pages on the fly. **WARNING** - official version of GreaseMonkey sends some data to their servers.
   * Useful user scripts (do **not install** without reviewing the scripts):
     * [Direct Google](https://greasyfork.org/en/scripts/568-direct-google) - Removes Google redirects and exposes "Cached" links.
     * [GitHub White NavBar](https://github.com/victor-li/github-white-navbar) - makes Github navigation bar white.
  * User script repositories:
    * [GreasyFork](https://greasyfork.org/)
    * [OpenUser.JS](https://openuserjs.org/)

 _A note on add-ons published by Mozilla: the review times are [spiking](https://blog.mozilla.org/addons/2017/02/14/add-ons-update-92/#comments)._
 
## Making workflow comfortable

 * [ScrapBook X](https://addons.mozilla.org/en-US/firefox/addon/scrapbook-x/) - an extension for bookmarking and wholesale saving page content for future perusal.
 * [LuciFox](https://addons.mozilla.org/en-US/firefox/addon/lucifox/) - an extension for reading e-books in Firefox.
 * [SQLite Manager](https://github.com/lazierthanthou/sqlite-manager) - creating, reading, updating etc. SQLite databases from within the browser.
 * [VimFx](https://github.com/akhodakivskiy/VimFx) - if you have ever wanted to use Vim keyboard shotcuts for browsing in Firefox.

## Restyling well-known sites
 
 * [Wide GitHub](https://github.com/xthexder/wide-github) - for those who don't like white space.
 * If you want to restyle _any_ site, you don't need any more extensions ([Stylish](https://github.com/JasonBarnabe/stylish) etc.) Simply edit [this gist](https://gist.github.com/Hunter-Github/446d8fd36899a7d9180a) and add it to GreaseMonkey to suit your case.

## Recovering passwords

While [you shouldn't keep passwords in Firefox](#hardening-your-firefox) sometimes you have to: 

* [LaZagne](https://github.com/AlessandroZ/LaZagne) - recovers passwords.

## Firefox clones/forks

_Mozilla is entering into partnerships with commercial entities (like Telefonica) and considering radically changing the API which may kill the browser and its ecosystem. This necessitates starting an early search for respectable substitutes._

* [PaleMoon](https://www.palemoon.org/) - GitHub repo is called [Pale-Moon](https://github.com/MoonchildProductions/Pale-Moon).
* [IceCat](http://www.gnu.org/software/icecat/) - a GNUish fork which unfortunately lags behind FF at the moment.
* [Mozilla Build Instructions](https://developer.mozilla.org/en-US/docs/Simple_Firefox_build) - the dev environment is huge.
* [Linux build pre-requisites](https://developer.mozilla.org/en-US/docs/Mozilla/Developer_guide/Build_Instructions/Linux_Prerequisites).

The easiest way to get a modern and performant browser, though, is switching to an ['unstable' Chromium](https://download-chromium.appspot.com/). Although it still requires some customization, it supports uBlock Origin/uMatrix.

## Where to look for other awesome lists

* [awesome-awesome](https://github.com/emijrp/awesome-awesome)  
* [awesome-awesomeness](https://github.com/bayandin/awesome-awesomeness)
* [sindresorhus/awesome](https://github.com/sindresorhus/awesome)
* [freshcode](http://freshcode.club/) - a re-incarnation of Freshmeat, a directory of open-source/free software, with update notifications available.


<sub>[!["Creative Commons License"](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)]((http://creativecommons.org/licenses/by-sa/4.0/)]) This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).</sub>
