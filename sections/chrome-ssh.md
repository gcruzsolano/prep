# Login with Chrome SSH Extension

Using the Chrome SSH Extension is another option—especially for
those with only Windows machines to use from home. This option
requires you to login to Google Chrome, (which is very hard to undo
once you have done it allowing others after you to delete bookmarks
and such), and connections are blocked by some organizations. Use
[CodeAnywhere](codeanywhere.md) when in doubt. This option also take
considerably more setup than CodeAnywhere. However, the SSH extension 
is faster and more secure than CodeAnywhere because it is a direct
SSH connection just like [Terminal](terminal.md) but from the browser.

**Teachers and Assistants:** Because this method frequently creates
problems with students messing up each other’s Chrome bookmarks,
Gmail, and more it is not good for classroom use. If you choose to
walk one or more students through the process **be sure to log them
out.** Despite good intentions this is repeatedly forgotten and
therefore has been dropped from the list of Prep skills, albeit still
valuable for more advanced students or students with only Windows
machines as home. Consider using an individual student’s *digital
recess* time to help them configure it if they need it from home.

## Login to Chrome, *Not* Just Gmail/Google

This is a little tricky. You need to login to your Chrome Browser
itself, not Gmail or Google+. This cannot be done, unfortunately, from
Incognito, which is why this is so problematic for students in
a classroom setting.

![](/assets/chrome-ssh1.gif)

## Install SSH Chrome Extension

Search for `chrome ssh` while logged into Chrome as yourself.

![](/assets/chrome-ssh2.gif)

## Add to Bookmarks

Adding the SSH app to your bookmarks makes it easy to login from
anywhere that you can login to Chrome.

![](/assets/chrome-ssh3.gif)

## Configure for `skilstak.sh`

Just type in your user name followed by `@skilstak.sh.` It will fill
in the rest. You don't need to change anything else about the
connection settings.

![](/assets/chrome-ssh4.gif)

## Solarize

As soon as you login you will likely notice the default is not
solarized. Never fear, we got you covered. Head over to
[`solarized.skilstak.io`](http://solarized.skilstak.io) and save the raw
`json` file.

![](/assets/chrome-ssh5.gif)

Then you will need to load this configuration file by clicking on
`Options.`

![](/assets/chrome-ssh7.png)

And then on `Restore Backup` and find the JSON file you downloaded in
the previous step.

![](/assets/chrome-ssh8.png)

This will solarize everything from that point on *and* stay with you
no matter where you use the Chrome SSH extension, (which could not be
said for PUTTY and other alternatives).

![](/assets/chrome-ssh6.gif)

---
[![home](/assets/home-bw.png)](/README.md)
[![cc-by-sa](/assets/cc-by-sa.png)][cc-by-sa]
[![skilstak](/assets/skilstak-logo-bw.png)][skilstak]
[cc-by-sa]: https://creativecommons.org/licenses/by-sa/4.0/
[skilstak]: http://skilstak.io

