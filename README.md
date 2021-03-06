# jquery.SplashScreen.js
Create Splash Screen for Website/Mobiles, splash screen will display till the webpage completes loading of the images.

How to use
----------

To get started, download the plugin, unzip it and copy files to your website/application directory.
Load files in the <head> section of your HTML document. Make sure you also add the jQuery library.

    <head>
        <script type="text/javascript" src="//code.jquery.com/jquery-2.1.3.min.js"></script>
        <link rel="stylesheet" href="jquery.SplashScreen.css" type="text/css" media="screen" />
        <script type="text/javascript" src="jquery.SplashScreen.js"></script>
    </head>

Initialise the script like this:

    <script>
        $(document).ready(function() {
            $.SplashScreen();
        });
    </script>

May also be passed an optional options object which will extend the default values. Example:

    <script>
        $(document).ready(function() {
            $.SplashScreen({
                id: 'splashscreen',
                desktop: true,
                mobile: true,
                forceLoader: false,
                queryParameter: 'loader',
                progressCount: false,
                progressCountId: 'status',
                progressBar: false,
                progressBarId: 'progress',
                fadeEffect: true,
                timeToFade: 1000, // in milliseconds (eg: 1000 = 1sec)
                timeOut: 2000   // in milliseconds (eg: 2000 = 2sec)
            });
        });
    </script>

Accepted querystring parameter values for forceLoader are as follows
- ?loader=true
- ?loader=t
- ?loader=1

Place the div before the closing of &lt;/body&gt;

    <div id="splashscreen">
        <!-- you can add your custoem preloader images etc.... -->
    </div> 

Tip: You can override CSS to customize the look.
