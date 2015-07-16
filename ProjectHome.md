

# What is YouTube Direct Lite? #

There are two parts two the YouTube Direct Lite platform: a submission widget, which can be embedded on any existing website, and a moderation interface for reviewing videos that have been submitted.

The submission widget allows anyone visting your site to upload a new video to their own YouTube account from their hard drive, record a new video using their computer's webcam, or to submit a video that they've already uploaded for review.

Each video submissions is tied to a specific YouTube playlist, but the videos are not added to the playlist immediately. The submissions need to be moderated first, and only videos that are approved are added to the playlist.

The moderation interface allows the owner of the playlist to approve or reject video submissions that are associated with that playlist. When a video is approved, it's added to that playlist. Rejecting a video moves it out of the list of videos waiting to be moderated, and the actual video remains active on YouTube.

# Why Should I Use YouTube Direct Lite? How Does it Compare to YouTube Direct? #

Adding YouTube Direct Lite is as simple as adding an iframe HTML tag to your existing web pages. There is no server-side code that needs to be configured or deployed, though we do recommend that you check out your own copy of the YouTube Direct Lite HTML/CSS/JavaScript and host it on your existing web server.

[YouTube Direct](https://code.google.com/p/youtube-direct/) is an existing open source project that provided much of the same functionality as YouTube Direct Lite. However, using it requires setting up a [Java App Engine](https://developers.google.com/appengine/docs/java/overview) server and the configuration process can be difficult for those not familiar with the environment.

If you are primarily a web master and do not have experience working with Java or App Engine, then adding YouTube Direct Lite to your site will be much more straightforward than using YouTube Direct.

YouTube Direct Lite does not allow you to collect additional metadata when soliciting videos, like the user's contact information or location. If that's a requirement, then you should use YouTube Direct. Also, if being notified as soon as possible when new videos are submitted is important, YouTube Direct is a better choice. For most other scenarios, though, YouTube Direct Lite is recommended for new integrations.

# Live Demo #

You can visit http://ytdirectlite.appspot.com/static-min/submit.html for a live demonstration of what the submission widget looks like and how it can be integrated onto a web page.

An example of YouTubeDirect Lite administration interface can be found at http://ytdirectlite.appspot.com/static-min/admin.html Note that it will not be that interesting unless you're moderating a playlist in your own YouTube account that has already had some videos submitted to it using YouTube Direct Lite.

# Important Caveats #
  * YouTube Direct Lite locates videos submitted to a specific playlist by searching for a specially formatted keywords that are added to all submissions. There is always a delay between the time a video is submitted and the time that it appears it searches for that keyword, as described in  the [YouTube API documentation](https://developers.google.com/youtube/2.0/reference#Latency_Information). This can mean a delay of minutes or even hours before a new submission shows up in the moderation interface.
  * YouTube playlists can only contain 200 entries. This is not a limitation of YouTube Direct Lite, but it's something to keep in mind since approved/rejected videos are stored in playlists.

# Other Clients #

In addition to the web-based submission method, there is an [open source Android reference implementation](https://github.com/youtube/yt-direct-lite-android) that you can modify to suit your needs.

# Next Steps #

The GettingStarted guide contains instructions on how to add YouTube Direct Lite to your existing website.