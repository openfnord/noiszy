# Noiszy


Noiszy is a plugin that creates meaningless web data by navigating your browser randomly around a list of sites, to confound tracking & personalization algorithms and burst filter bubbles.

Learn more about this project at [noiszy.com](https://noiszy.com/) and the [Noiszy blog](https://noiszy.com/blog/).

## Open source - here we go

  - By popular demand, we're going open source.
  - This is my first open-source project, so helpful comments will be greatly appreciated.

## A note about tracking
As explained on the [privacy page of noiszy.com](https://noiszy.com/privacy/), we are tracking Noiszy usage with Google Analytics.  This lets me know how many people are using Noiszy, and how much data they're generating.  I completely understand that some people will be bothered that Noiszy tracks anything, but the point of Noiszy is to create data, and to spur the conversation about what should then be done with that data.  I believe that knowing amounts of data from Noiszy is useful and reasonable, and it's done transparently - so I stand behind this.  Of course, debate is welcomed.  At any rate, you'll find some GA snippets in the code.

Hopefully, I managed to remove Google Analytics.

Noizy can be used to produce "natural" web traffic. Here the timing needs to be adjusted in background.js :231 base_interval = 0.01 instead of 1

## Testing with firefox.
one can unpack the xpi (it is a zip) and replace the files in the archive with the html and js files of this repo and zip it again and call it .xpi

The META-INF directory needs to be removed as this is not signed anymore.

In the browser in about:config the setting "xpinstall.signatures.required" needs to be set to false to allow the installation of unsigned extensions (use with care!)

You can use the test_noiszy.xpi which includes the newest modifications but is unsigned at the moment. I need to find out how to sign firefox extensions.
