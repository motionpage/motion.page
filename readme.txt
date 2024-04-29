=== Motion.page ===
Author URI: https://motion.page
Plugin URI: https://motion.page
Contributors: Rados51, DavidBabinec, krzysztoff1
Tags: motion, animations, gsap
Requires at least: 5.8.6
Tested up to: 6.5.2
Requires PHP: 7.4
Stable tag: 2.1.8
License: EULA + GPLv2
License URI: https://motion.page/eula

Move it like it's HOT!

== Description ==

With Motion.page for WordPress, you can animate anything you can imagine without writing a single line of code, in a fully visual builder.

== Installation ==

After the purchase of one of our plans, download the plugin from the member's area, and follow the basic process.

1. Download the plugin
2. Install the plugin by uploading the zip file to Plugins > Add New
3. You will see the new "Motion.page" link at bottom of the WP sidebar, which launches the builder
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

= 2.1.8: 30-04-2024 =
* [new] From/To custom code field allows the use of MorphSVG plugin
* [fix] Motion Path validation schema - use default type if value is invalid
* [fix] Safari builder page refresh issue
* [fix] Remove other instances of GSAP - works only if there are activate timelines on the page
* Various minor tweaks, bug resolutions and additional improvements

= 2.1.7: 30-03-2024 =
* [new] Remove other instances of GSAP library on the frontend [Experimental]
* [tweak] Image Sequence - offload images loading to the Worker thread
* [tweak] Image Sequence Transcoder - multi-threaded transcoding for faster processing
* [tweak] Image Sequence Transcoder - support Arc browser and Firefox version >= 119
* [tweak] Two new PHP filters (motionpage/utils/disableMobile & motionpage/utils/gsapDeferAsync)
* [tweak] Scripts and files should have better exclude support for optimization plugins
* [tweak] ScrollTrigger refresh script transpiled as ES6
* [tweak] Faster post/page fetching in the builder
* [tweak] Remove new post types from WP 6.5, that are not needed in the builder
* [tweak] SelectorScanner will look for a unique parent selector for Breakdance images
* [tweak] Lottie integration now supports also dotLottie
* [fix] Save Button - incorrect behaviour on Mouse Movement trigger
* [fix] Additional selectors in the generated code for ScrollTrigger start/end (in rare cases)
* [fix] ScrollSmoother option "Move fixed elements outside the wrapper" issue with Bricks builder
* [fix] Global Settings config loss during the site migration
* [fix] Data validation issue caused by empty "Offset from element" input field in Image Sequence
* [fix] No Posts error notice on empty Oxygen templates
* [fix] Three missing tooltips
* [fix] NumPad Enter should work as Enter in the builder
* [fix] Prevent "Cookie Yes" to show in the builder iframe
* [fix] Replace FILTER_SANITIZE_STRING with htmlspecialchars for better PHP 8.1 compatibility
* [fix] Prevent error #011 when the issue is non-existent
* [fix] Timeline playhead component - issue with the playhead position
* [fix] ClickCopy - better compatibility with different browsers
* [upgrade] GSAP 3.12.5
* Various minor tweaks, bug resolutions and additional improvements

= 2.1.6: 06-11-2023 =
* [tweak] Three new PHP filters
* [tweak] Exclude Motion.poge files from Speedien plugin (Nestify)
* [fix] Page Exit code rendered by accident on the frontend (in some cases)
* [fix] LazyLoaded browser event - refresh script disabled by default

= 2.1.5: 21-10-2023 =
* [fix] Split Text missing in the actual code (in some cases)
* [fix] ScrollTrigger Custom Code Field - issue with nested objects
* [fix] ScrollTrigger pin hanging in DOM after removal (in some cases)
* [fix] Exclude Motion.page from Page Optimize plugin
* [fix] Prevent Image Sequence from loading in ARC browser (as it is not supported by the browser)

= 2.1.4: 08-10-2023 =
* [fix] Wrong number of parameters in the plugin action links

= 2.1.3: 07-10-2023 =
* [tweak] ScrollTrigger refresh function hooked to document lazyloaded event
* [tweak] Optimole compat layer
* [fix] WP Meteor compat layer
* [fix] Save button duplicate action

= 2.1.2: 20-09-2023 =
* [fix] Error #002A | #002B that impacted specific server configurations
* [fix] Incorrect styling of the update notice

= 2.1.1: 16-09-2023 =
* [fix] Zod data validation schema

= 2.1.0: 14-09-2023 =
* [new] Mouse Movement
* [new] MotionPath integration
* [new] Client Mode
* [new] Zoom/Unzoom timeline component
* [new] ScrollTrigger clamp
* [new] ScrollSmoother speed option
* [new] Smooth scroll to hash anchor on page load
* [new] Better WPML & Polylang support - sync timelines across all languages (UI toggle)
* [new] Disable ScrollSmoother on frontend for admin users (UI toggle)
* [new] Page Events are wrapped with gsap.context
* [tweak] Database table split into two tables
* [tweak] Image Sequence- Support for WebP as a transparent image format
* [tweak] Image Sequence - Device Pixel Ratio
* [tweak] Display spinner component during deletion of image sequence files
* [tweak] Use 'motionpage/action/front' to confirm plugin's frontend activity
* [tweak] Option to hide quick action link (Edit with Motion.page)
* [tweak] Ease dropdown indicates that users can either select or input the ease
* [tweak] Improved code compression in certain scenarios
* [tweak] Option to change license key by holding down arrow key during builder launch
* [tweak] Updated icon for the timeline visibility toggle
* [tweak] License keys are hashed in the database
* [tweak] Smooth anchor links support URLs starting with '#' or '/#'
* [tweak] Image Sequence - image decoding attribute set to async during lazy load
* [tweak] Better multi-site support
* [tweak] Image Sequence supports .mov and .webm files
* [tweak] Additional filters in the library
* [fix] UI displays consistent breakpoint values as saved ones
* [fíx] Custom Transition plugin supports transition CSS property
* [fix] Resolved timeline duplication inconsistencies
* [fix] Load CustomEase plugin when gsap.parseEase is used in the custom code field
* [fix] Posts API returns an empty array if no posts are available
* [fix] Quick action link (Edit with Motion.page) loads the correct iframe URLs
* [fix] Custom Code Field resolved function name issues
* [fix] Generated code compiles to ES2015 (ES6) instead of ES2016
* [fix] Proper license removal upon uninstallation
* [UI] Introduced new sections in global settings
* [UI] Slider adjusts value with mouse click-n-drag
* [upgrade] GSAP 3.12.2
* Various minor tweaks, bug resolutions and additional improvements

= 2.0.0: 16-02-2023 =
* [new] Redesigned UI
* [new] Light theme
* [new] Image Sequence + Video transcoder
* [new] SplitText
* [new] Custom code block in ScrollTrigger and From/To properties
* [new] Modify/edit selector with the right-click
* [new] Sticky/Fixed elements are automatically moved outside of ScrollSmoother wrapper
* [new] Image Sequence Shortcode [mp-canvas]
* [new] Remove all data and license on uninstall, can be enabled from the Builder Settings pane
* [new] Opt-in for receiving Beta releases from the Builder Settings pane
* [new] ScrollTrigger custom code field allows the use of ScrambleText plugin
* [new] CookieBot compatibility with motionpage/utils/cookieconsent filter
* [new] Sync Motion.page iframe reload with Elementor save button (same page)
* [new] Quick Action Links in the admin
* [tweak] All generated code is ES6 compatible
* [tweak] ScrollSmoother won't run on mobile devices if touch is set to zero
* [tweak] Hide full license key in login screen
* [tweak] Lower memory consumption during posts/pages fetching (~8% less)
* [tweak] Increase memory limit for post/pages fetching on excesive posts/page count
* [tweak] Flush permalink rewrite rules on plugin activation and update
* [tweak] Support for rem, em, vh, vw, vmin, vmax units in Translate and Dimensions
* [tweak] Support for "center" in ScrollTrigger element positions
* [tweak] Optimized PHP code loading / performance
* [tweak] Initiate SelectorDetector on input focus
* [tweak] SelectorDetector disables when selector is added by pressing an enter key
* [tweak] Hide invalid selectors in SelectorDetector
* [tweak] Show notice on timeline show / hide toggle from library tab
* [tweak] Show diod indicator if any values are enabled in advanced targeting/options
* [tweak] Timeline shows "No page assigned" instead of spinner if the page ID is not found
* [tweak] Hide Repeat / Stagger icon from timeline if the value is set to 0
* [tweak] 0019 issue notice explains how to fix the issue
* [tweak] Wordpress filters - naming consistency
* [tweak] Close builder dropdowns on scroll
* [tweak] Tooltips positioning
* [tweak] Suggested selectors in Lottie
* [tweak] ScrollTrigger ToggleActions - hide selected option in the dropdown
* [fix] Breakpoints settings (new range option)
* [fix] Timeline node drag and resize issues
* [fix] In some cases, there was need to click twice to play the timeline
* [fix] Issue with importing timelines from other sites
* [fix] Bypass reduced motion state on toggle
* [fix] Range slider input component
* [fix] Error when stagger value is changed back to 0
* [fix] ScrollTrigger Pin issue
* [fix] Allow 0 as a value inside Filters
* [fix] Missing timeline trigger on individual timelines if trigger was empty
* [fix] Number inputs correct values during initialization
* [fix] Missing builder CSS polyfills for older browsers
* [fix] Modals work correctly in Safari and Firefox
* [fix] Proper handling of unsupported browsers in the builder
* [fix] Incorrectly loaded builder CSS on specific server configs
* [fix] Long selector badge
* [fix] Multiple export/delete from library
* [fix] Missing Oxygen template in some cases in advanced targeting
* [upgrade] GSAP 3.11.4
* [deprecated] Dropped support for PHP version lower than 7.4
* [lib] Removal of Chakra Number Inputs
* Various minor changes, bug fixes and additional improvements

= 1.6.7: 31-01-2023 =
* [fix] Issue with the builder not loading after downgrading to 1.6.6 from 2.0.0
* [fix] Issue with removing multiple timelines from library
* [fix] Incorrect unit switch

= 1.6.6: 25-10-2022 =
* [fix] Node duration change not working correctly in some cases
* [fix] Advanced targeting (Oxygen template) not loading correctly for logged-out users
* [fix] ScrollTrigger timeline repeat YoYo effect - incorrectly generated value

= 1.6.5: 24-10-2022 =
* [tweak] Possibility to write down any ease in the easing dropdown
* [tweak] Less code on the front-end
* [tweak] SiteGround Optimizer compatibility - Auto exclude list/function
* [tweak] ScrollTrigger offset position values
* [fix] ScrollSmoother - loading corrected on pages without ScrollTrigger
* [fix] ScrollSmoother - disabled reactivation after value change
* [fix] Timeline component node - incorrect values after browser zoom in/out
* [fix] Prevent builder breakage if wp_debug outputs a warning inside the API request (PHP 8.1.9)
* [fix] PHP warning that emerged after post fetch
* [lib] Removal of Axios library

= 1.6.4: 23-09-2022 =
* [fix] Lottie selectors accepts IDs and classes correctly
* [fix] _mp_refresher uses global window variable
* [downgrade] GSAP 3.10.4

= 1.6.3: 13-09-2022 =
* [ui] Left panel overlay during iframe URL change
* [fix] ScrollTrigger refresh function
* [fix] Wrong values during nodes switching

= 1.6.2: 06-09-2022 =
* [new] Possibility to use RegEx inside Advanced Targeting
* [tweak] Possibility to animate CSS variables in Custom value fields (scans root, HTML & body for CSS variables)
* [tweak] Resize the timeline by grabbing any point at the top
* [tweak] Possibility to use days property inside mp-block shortcode (default is 30)
* [tweak] Auto exclude GSAP files from WP-Rocket (with rocket_delay_js_exclusions filter)
* [tweak] Possibility to use _mp_refresher function, which will sort and refresh all ScrollTriggers on the page
* [tweak] Query parameters /?mp=preview or /?mp=dbid1 bypass reduced motion
* [ui] Expand animation selector input on focus
* [ui] Wider value fields for custom and filter properties
* [fix] Browser's back and forward buttons on page exit triggered timelines
* [fix] Using double quotes in selector inputs without breaking
* [fix] Iframe refresh on page select
* [fix] Timeline playhead issues
* [fix] Non-working filters in UI
* [update] GSAP 3.11.1
* Various minor changes, fixes, and improvements

= 1.6.1: 20-08-2022 =
* [fix] Issue with iframe loading on specific sites

= 1.6.0: 19-08-2022 =
* [new] Lottie
* [new] DrawSVGPlugin
* [new] Select colors with Eye Dropper (works with HTTPS and the latest Chromium browsers)
* [new] mp-block & mp-unblock shortcodes - allow users to block timelines on frontend
* [new] Preview timelines on frontend via URL query [e.g. /?mp=dbid1 || multiple split with - or ,]
* [tweak] Faster loading time of the builder
* [tweak] Possibility to use a different selector for the 2nd click for the click event
* [tweak] Possibility to use multiple filters
* [tweak] ScrollSmoother refresh function after page load
* [tweak] Possibility to close SelectorDetector with ESC key
* [tweak] Exit browser notice if there is an unsaved timeline
* [tweak] CloudFlare rocket loader - cfasync=false attribute for all GSAP files
* [fix] Suppress PHP warnings when the database is not up-to-date with a builder
* [fix] Non-working Hue Rotate filter
* [fix] Non-working Border Color
* [fix] Background Position
* [fix] Wrongly displayed viewport units on first load inside UI
* [fix] Correct license input field on new installations
* [fix] Prevent duplicate IDs on import
* [fix] Timeline playhead issue
* [fix] Markers disappearing or at wrong positions
* [ui] Split From / To properties to Visual and Functional
* Various minor changes, fixes and improvements

= 1.5.2: 31-05-2022 =
* [fix] Versioning system & Update system

= 1.5.1: 25-05-2022 =
* [fix] ScrollSmoother input resulting in black screen
* [fix] Prevent black screen if builder loading takes longer

= 1.5.0: 23-05-2022 =
* [new] ScrollSmoother plugin
* [new] 3D Transform property
* [new] Page Exit triggered by specific selectors
* [new] Sync Motion.page iframe reload with Oxygen or Bricks save button (same page)
* [new] Timeline repeat delay option
* [new] Disable post types inside builder
* [tweak] Speed improvements on post fetching
* [tweak] Loader overlay if action might take longer then expected
* [fix] Advanced targeting not properly working in some cases
* [ui] Settings moved to a top-right panel
* [ui] Feature request button/link
* [update] GSAP 3.10.4
* Various minor changes, fixes and improvements

= 1.4.1: 30-03-2022 =
* [fix] Wrong PHP condition when all of the timelines are set to bypass reduced-motion

= 1.4.0: 29-03-2022 =
* [new] Target timelines by the Post Type, Oxygen templates or URL
* [new] Filter timelines in the library
* [new] WordPress multisite support
* [new] Repeat / Loop the whole timeline
* [new] From / To context menu on right-click [Duplicate, Toggle, Clear, Copy, Paste]
* [new] Pause "page load" event timelines before execution
* [new] Custom PHP filters for targeting timelines content and execution
* [new] Ease in the custom property now accepts cubic-bezier or path string values
* [new] Hover - restart timeline on mouse leave
* [new] Option to bypass 'prefers-reduced-motion' for a single timeline
* [tweak] Remove JetEngine data-url attributes and prevent click inside the builder
* [tweak] Custom Toggle Actions
* [tweak] Toggle Actions new property "play reverse play reverse" [Always reverse on scroll backwards]
* [tweak] Highlight timeline name on library right click
* [tweak] Auto-scale timeline component preview length if the timeline is longer than the preview length
* [tweak] Better error handling (notice in the bottom right corner)
* [tweak] Prevent page exit timeline by targeting wrapper parent (#wrapperID.ignore-exit)
* [tweak] Ease & Filter - search by typing
* [tweak] Imports with different post ID are assigned to homepage ID on change from the library
* [fix] Plain Permalinks compatibility
* [fix] ScrollTrigger start/end offset issue
* [fix] Ease removal issue + correct naming
* [fix] Timeline component preview length is now saved together with the timeline
* [fix] Timeline playhead bounds area
* [fix] Prevent playhead move upon activating different timeline from the library
* [fix] Scroller markers disappeared after iframe refresh
* [fix] Piotnet Grid post fetching
* [fix] Unsaved timeline not working correctly after iframe reload
* [fix] Safari Repeat (yoyo) toggle bug
* Various minor changes, fixes and improvements

= 1.3.0: 24-01-2022 =
* [new] ScrollTrigger - Play each iteration of the class individually when triggered
* [new] Copy timeline UID from context menu in the library
* [tweak] Prevent builder from breaking if selector is not a valid DOM selector
* [tweak] Excluded classes for the Exit trigger can be pasted with and without dot
* [tweak] Custom API for fetching all posts by post type name
* [tweak:fix] Allow multiple selectors as Click / Hover triggers
* [tweak:fix] Usage of optional chaining for event listeners which prevents code breaking
* [fix] WordPress 5.9 compatibility

= 1.2.2: 11-01-2022 =
* [tweak] ScrollTrigger refresh and sort function
* [fix] After Load Page Event

= 1.2.1: 03-01-2022 =
* [update] GSAP 3.9.1
* [fix] Playhead tied to old timeline
* [fix] Wrongly generated click/hover selector in some cases

= 1.2.0: 02-01-2022 =
* [new] Click / Hover - Play each iteration of animated class individually when triggered
* [new:tweak] Allow timeline restart on Click event
* [tweak:breaking] A timeline node without selector takes previous selector instead of the first one
* [tweak] Scale value is possible to increment by 2 decimals
* [tweak] Suppressed warnings in the console
* [fix] It's not possible to place animation node outside of the timeline anymore
* [fix] Wrong position in the code for Click/Hover trigger - thus not working properly
* [fix] Translate/BGPosition/Dimensions values/units bug
* [fix] Breakpoints not working in some cases
* [fix] Interactions Click/Hover dropdown bug - wrongly selected trigger after opening existing timeline
* [fix] Custom property works again with a comma separated array
* Various minor changes, fixes and improvements

= 1.1.2: 17-12-2021 =
* [fix] Builder will not break during invalid selector
* [fix] Weird issue with vendors file names

= 1.1.1: 16-12-2021 =
* [tweak] Additional SrollTrigger.refresh function that prevents misorder of pined timelines
* [tweak:fix] Activate site with http/s prefix inside EDD to prevent domain name mismatch
* [fix] Rotation value set to 0 was shown like empty input
* [fix] Unnecessary DOMContentLoaded listener wrap on Page Load timelines

= 1.1.0: 11-12-2021 =
* [new] Possibility to use pin in ScrollTrigger
* [new] Adds "play none none reverse" to toggle actions as Reverse on scroll back leave
* [new] If prefers-reduced-motion is set to reduce, timelines will not execute on the frontend
* [tweak] Disable timeline restart after save
* [tweak] Page exit ignored selector not preventing default click (event) action
* [tweak] Possibility to use multiple classes as ignored page exit selector (split by comma)
* [tweak:fix] Remove visibility:hidden inside iframe (possibility to use body as selector in FromTo)
* [fix] Prevent unnecessary re-renders inside builder
* [fix] Timelines stacking (in some cases)
* Various minor changes, fixes and improvements

= 1.0.9: 02-12-2021 =
* [fix] Possibility to open timeline with non-existing post
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
* Birthday of Motion.page & this readme.
