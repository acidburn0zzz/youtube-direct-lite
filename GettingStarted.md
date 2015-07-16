

# Local Deployment vs. Using Reference Instance #

YouTube Direct Lite consists of pure HTML, CSS, and JavaScript. There is no server-side code. As such, it can be hosted on any standard web server.

The biggest decision to make before you start using YouTube Direct Lite is whether you want to host a copy of the HTML/CSS/JavaScript on your own web server, or simply add a reference to the version of YouTube Direct Lite being served off of `ytdirectlite.appspot.com` to your web pages.

The instructions for using YouTube Direct Lite vary depending on which approach you take, and the following information can help you decide.

# You Should Use a Local Deployment If... #

  * Pages that host YouTube Direct will receive significant traffic. If you run a popular website, we ask that you host your own copy YouTube Direct Lite instead of using the reference instance.
  * You need to customize the submission interface. Once you check out a copy of the HTML/CSS/JavaScript, you have full control over changing the widget's user interface or color scheme to match that of your website.
  * You want complete control over updating the code. You can pull the latest updates from the central code repository and deploy them to your web server on your own schedule. If you use the reference instance, the behavior or interface of the widget will change whenever new code is pushed out by YouTube Direct Lite's maintainers.

# You Should Use the Reference Instance If... #

  * You do not have the ability to deploy arbitrary HTML/CSS/JavaScript files on the web server that hosts your site. You might be running your site on a third-party hosting platform, for instance.
  * You're not comfortable checking out files from a Git repository or adding them to your local web server.
  * You do not need to customize the default YouTube Direct Lite interface or modify the code.
  * You would prefer to have immediate access to any bug fixes or feature enhancements that are added to YouTube Direct Lite.

# Next Steps #

Follow the instructions for HostingYourOwnInstance or using the ReferenceImplementation.