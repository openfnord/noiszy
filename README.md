# Noiszy


Noiszy is a plugin that creates meaningless web data by navigating your browser randomly around a list of sites, to confound tracking & personalization algorithms and burst filter bubbles.

Learn more about this project at [noiszy.com](https://noiszy.com/) and the [Noiszy blog](https://noiszy.com/blog/).

## Open source - here we go

  - By popular demand, we're going open source.
  - This is my first open-source project, so helpful comments will be greatly appreciated.

## A note about tracking

I managed to remove Google Analytics, you do not want to be tracked, period.


## Timing
The timing can be adjusted in background.js: base_interval = 0.01 instead of 1. Use 1 for more human browsing and entertainment as you have about 1 minute left for reading. Use 0.01 for traffic generation.
In the future there will be a parameter in the settings (options.html and options.js) to configure the base_interval of background.js which is used as factor for random number timing.

## Testing with firefox.
one can unpack the xpi (it is a zip) and replace the files in the archive with the html and js files of this repo and zip it again and call it .xpi

The META-INF directory needs to be removed as this is not signed anymore.

In the browser in about:config the setting "xpinstall.signatures.required" needs to be set to false to allow the installation of unsigned extensions (use with care!)

You can use the test_noiszy.xpi which includes the newest modifications but is unsigned at the moment. I need to find out how to sign firefox extensions.

The test_noiszy.xpi has hard coded timing for traffic generation.
