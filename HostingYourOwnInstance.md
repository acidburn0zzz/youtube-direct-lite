

# Introduction #

So you've decided to host your own instance of YouTube Direct Lite—great! The following guide will walk you through all the steps needed to get up and running.

# Prerequisites #

  * A [git client](http://git-scm.com/downloads) to check out the code.
  * Administrative access to any type of web server.

# Checking out the Code #

From the command line, navigate to a directory that's being served by your web server, and clone the YouTube Direct Lite project using `git`. For the purposes of this example, we'll assume that's `/var/www/`, though the actual directory you should use is specific to your web server.

```
cd /var/www
git clone https://code.google.com/p/youtube-direct-lite
```

This should create a local `youtube-direct-lite` directory that will be hosted by your web server.

# Configuring the Code #

There are two required changes that you must make to a JavaScript file, [config.js](https://code.google.com/p/youtube-direct-lite/source/browse/static/js/ytdl/config.js), before you can use your local instance of YouTube Direct Lite.

Open `youtube-direct-lite/static/js/ytdl/config.js` in your preferred text editor, and follow the instructions in the comments for generating your own `OAUTH2_CLIENT_ID` and `DEVELOPER_KEY` and add them to the file.

There are other optional configuration changes that you can make to this file as well. The comments in the file explain more.

# Customize Your Interface #

Take the time to modify the HTML, CSS or JavaScript that you've downloaded to suit the look and feel of your web site.

# Staying Up to Date #

If you'd like to update to the latest YouTube Direct Lite codebase at any point in the future, you can do so by running

```
git pull
```

from within your `youtube-direct-lite` directory. If you've made any modifications to your local HTML, CSS, or JavaScript, you'll have the merge your changes with the changes pulled down from `git`.

**Important**: It is recommended that you join [this mailgroup](https://groups.google.com/forum/?fromgroups#!forum/ytdl-code-pushes) to receive notifications when new code is submitted. This will give you a good idea as to when you need to pull in the latest release to your local repository.

# Next Steps #

Learn about accessing the AdminInterface so that you can generate an iframe embed code, as well as moderate videos that have been submitted.