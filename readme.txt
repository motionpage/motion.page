=== motion.page ===
Author URI: https://motion.page
Plugin URI: https://motion.page
Contributors: Rados51, DavidBabinec
Tags: motion, animations, gsap
Requires at least: 5.7
Tested up to: 5.9 RC 2
Requires PHP: 7.1
Stable tag: 1.2.3
License: EULA + GPLv2
License URI: https://motion.page/eula

Move it like its HOT!

== Description ==

With motion.page for WordPress, you can animate anything you can imagine without writing a single line of code, in a fully visual builder.

== Installation ==

After the purchase of one of our plans, download the plugin from the member's area, and follow the basic process.

1. Download the plugin
2. Install the plugin by uploading the zip file to Plugins > Add New
3. You will see the new "motion.page" link at bottom of the WP sidebar, which launches the builder
4. Launch the builder, and add your license key on the welcome screen, to activate it.

== Frequently Asked Questions ==

= How does this plugin work? =

It's a motion builder packed with powerful features. It brings a world of professional web animation into WordPress, with a UI that provides a smooth workflow. Install the plugin, launch the builder and animate any page from your site!

= What can I do with it? =

Create a simple animation or a complex timeline with multiple elements animated at different times. Attach your animation to prebuilt triggers like on load, page exit, scroll, click or hover, and create the ultimate website experience without writing any code.

= Does it affect performance? =

Motion.page was built with performance in mind from day one. Assets are conditionally loaded only on pages where they are used. It doesn't add more code than manually coded animations.

= What about CLS? =

Cumulative Layout Shift (CLS) will not be affected on any animated elements above the fold. If animations use transform properties, they are perfectly ok for Core Web Vitals.

== Changelog ==

= 1.2.3: 12-01-2022 =
* [fix] Issue with WordPress 5.9

= 1.2.2: 11-01-2022 =
* [tweak] ScrollTrigger refresh and sort function
* [fix] After Load Page Event

= 1.2.1: 03-01-2022 =
* [update] GSAP 3.9.1
* [fix] Playhead tied to old animations
* [fix] Wrongly generated click/hover selector in some cases

= 1.2.0: 02-01-2022 =
* [new] Click / Hover - Play each iteration of animated class individually when triggered
* [new:tweak] Allow animation restart on Click event
* [tweak:breaking] A timeline node without selector takes previous selector instead of the first one
* [tweak] Scale value is possible to increment by 2 decimals
* [tweak] Suppressed warnings in the console
* [fix] It's not possible to place animation node outside of the timeline anymore
* [fix] Wrong position in the code for Click/Hover trigger - thus not working properly
* [fix] Translate/BGPosition/Dimensions values/units bug
* [fix] Breakpoints not working in some cases
* [fix] Interactions Click/Hover dropdown bug - wrongly selected trigger after opening existing animation
* [fix] Custom property works again with a comma separated array
* Various minor changes, fixes and improvements

= 1.1.2: 17-12-2021 =
* [fix] Builder will not break during invalid selector
* [fix] Weird issue with vendors file names

= 1.1.1: 16-12-2021 =
* [tweak] Additional SrollTrigger.refresh function that prevents misorder of pined animations
* [tweak:fix] Activate site with http/s prefix inside EDD to prevent domain name mismatch
* [fix] Rotation value set to 0 was shown like empty input
* [fix] Unnecessary DOMContentLoaded listener wrap on Page Load animations

= 1.1.0: 11-12-2021 =
* [new] Possibility to use pin in ScrollTrigger
* [new] Adds "play none none reverse" to toggle actions as Reverse on scroll back leave
* [new] If prefers-reduced-motion is set to reduce, animations will not execute on the frontend
* [tweak] Disable animation restart after save
* [tweak] Page exit ignored selector not preventing default click (event) action
* [tweak] Possibility to use multiple classes as ignored page exit selector (split by comma)
* [tweak:fix] Remove visibility:hidden inside iframe (possibility to use body as selector in FromTo)
* [fix] Prevent unnecessary re-renders inside builder
* [fix] Animations stacking (in some cases)
* Various minor changes, fixes and improvements

= 1.0.9: 02-12-2021 =
* [fix] Possibility to open animation with non-existing post
* [tweak] Show "Missing Post ID / Title" instead of a spinner on non-existing post

= 1.0.8: 30-11-2021 =
* [fix] Some values was not removed in from/to
* Overcome EDD Unauthorized error by clicking on update badge (when update is available)
* Changed exported code when using both from and to (gsap.fromTo)
* Various minor changes and fixes
* Update GSAP to 3.8.0 (from 3.7.1)

= 1.0.7: 29-11-2021 =
* [fix] Confirm button loading state
* Various minor changes and fixes

= 1.0.6: 27-11-2021 =
* [fix] Prevent 40X errors due to server firewall

= 1.0.5: 27-11-2021 =
* [fix] Variable typo causing PHP Warning

= 1.0.4: 27-11-2021 =
* [partial-fix] CPTs filtering results in black screen

= 1.0.3: 26-11-2021 =
* Fixed CSS styling

= 1.0.2: 25-11-2021 =
* Possibility to add custom property inside From/To
* Disabled XYC shortcuts which in some rare cases randomly switched Builder/Settings
* It's possible to use space again in the input selector for advanced selector modifiers
* Fixed issue which breaks the builder during scroller input typing
* Iframe body color should inherit page body settings or use basic white color
* Welcome screen library duplicate option will close the welcome screen
* Disabled context menu (right-click), where not needed
* Console error if the site has disabled REST API
* Console warning if the site does not have a static page as a homepage
* Unnecessary load of inline code carrier — now tied to GSAP enqueue
* Unnecessary load of wpack.io script/text on the frontend
* Various minor changes and fixes

= 1.0.1: 22-11-2021 =
* Quick Fix

= 1.0.0: November 22, 2021 =
* First Release

= 0.0.0: January 11, 2021 =
* Birthday of motion.page & this readme.