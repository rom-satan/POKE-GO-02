PGMSuite

*pogomap site enhancements
What it does

    Adds support to filter IVs in a very basic way.
    Adds support to post to Discord when it sees a new Pokemon.

WARNING: If Discord posts are enabled it will post every Pokemon it sees to Discord! If filters are turned off on the site and the IV filters are too low the Discord updates will quickly become overwhelming, and Discord will rate-limit you meaning some Discord updates will vanish.
How to use
Basic Setup

    Download PGMSuite_user.js
    Install a userscript manager if you do not already have one. My recommendations: TamperMonkey for Chrome GreaseMonkey for Firefox
    Load PGMSuite_user.js
    Refresh the pogomap site.
    If you wish to use the Discord notifications, read point 4 Webhook URL below.

Each element

    Enable Discord By default this is unticked so that the initial site load will not spam your channel unnecessarily. Tick this checkbox to receive Discord updates to the webhook URL you supply. At the moment this fails silently, and can be rate limited so be careful when using it, but it should post to Discord everything you can see on your screen.
    IV % Change the value to set the lower bound of IV percentages you want to display for all Pokemon. This does NOT affect the Pokemon you have ticked to see in the site's Filter list (Dragonite, Snorlax etc).
    IV filter everything Tick this checkbox for the IV filter to apply to everything included the Filter Pokemon.
    Webhook URL This is the URL of your discord channel so that Pokemon can be posted there. This is the only element that will save and re-load between sessions. See more about webhooks here. Once you have set-up the filters and 'watching area' to your liking, you can tick the Enable Discord checkbox and Discord notifications will begin for newly appearing Pokemon.

Changelog
1.0.7

Skipped a version. Getting it working on Edge/IE, added CP to discord notification, better filtering without IV values.
...

Don't remember
1.0.2

Fixed IV filters not being inclusive with the value you input, e.g. 100% would never return anything.
1.0.1

Fixed 'filter everything' not being remembered.
