This repository is maintained by Cowboysdude and tbbear [SPECIAL THANKS FOR FOR ALL THE HARD WORK!]
[This is the second version of this module for MagicMirror2]

# MMM-NOAA

**Weather for your mirror**
  Also UV index and Air Quality Index.  [Warning AQI may not work in all areas if not then disable see config options].

## Examples

![](NOAA.PNG) 

If you do not enter a name in the config.js file it will just say either "Good Morning", "Good Afternoon" or "Good Evening".  With a name.  **** NEW UPDATE:  MUST ADD POSITION to config see example BELOW in sampe CONFIG ****
*Shows forecast or not, config option
*NO longer need to enter Lat and Lon... it's automatic!
*Automatically adjusts languge based on your config.js!

## Your terminal installation instructions

* `git clone https://github.com/cowboysdude/MMM-NOAA` into the `~/MagicMirror/modules` directory.
*  `~MagicMirror/modules/MMM-NOAA`
*  `npm install`

## Get your free API key here [WEATHER, You must also get an AirAPI Key--- see below]

 [https://www.wunderground.com/weather/api](https://www.wunderground.com/weather/api)

* Select the middle plan

## Get your PWS from here


 [https://www.wunderground.com/wundermap](https://www.wunderground.com/wundermap)
 
* For your config.js entry for precise localized weather 

## Get your AirKEY from here

 [https://airvisual.com/api](https://airvisual.com/api)

## Config.js entry and options

Will automatically select translation file and either F or C by reading your defaults from the config.js file [at the top]
Will default to EN if NO translation file is found.  Weather alerts will be in the native language chosen by your config.js automatically and in the correct language!  Thanks tbbear!!!

    {
        disabled: false,
        module: 'MMM-NOAA',
        position: 'top_right',
        config: {

		apiKey: "YOUR API KEY",    // https://www.wunderground.com/weather/api  select the middle plan... 
		useAir: false,             // set to false if you do not want to use Air Quality Index
		airKey: "YOUR API KEY",    // IF you want Air Quality Index
		pws: "KNYELMIR13",         // go here to find your pws: https://www.wunderground.com/wundermap
		showClock: true,           // Hides or shows clock
		dformat: true,             // for M/D/YYYY format, false for D/M/YYYY
		format: "12",              // 12 or 24 hour format.. will default to 12 hour if none selected.
		ampm: true,                // to show AM and PM on Sunrise/Sunset time
		showGreet: false,          // deafult is false - to show greeting under clock and above date
		name: "",                  // Your name
		showWind: false,
		showDate: false,
		showForecast: true,         //show bottom 3 day forecast
		flash: true,                 //Today in forecast flashes halo
		showUV: true,               //show UV index
	        showBar: true,             // show Barometer
	        showHum: true,              //show Humidity level
		position: 'top_right',       //whatever you have in above position must also be here
	        alert: true,                //show weather alerts default is true
		days: "3"                   //default in config is 3 can be either "3" or "10" for forecast
	}
    },

## Start your mirror . . . enjoy! 
