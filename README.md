# MicroFruit
MicroFruit Docs

Hi! And thanks for using the MicroFruit, built by Ben Strout. The MicroFruit is a small desk companion which will update the time, provide a weather forecast for a defined city, and tell you the time. In order to start using your MicroFruit though, you'll need to set up Wifi. You should see something like this when you first plug it in with the supplied USB cable.

The device will create a WiFi hotspot you can connect into named 'MicroFruit'. You should see this in your Wifi hotspot list:

![](RackMultipart20221224-1-9tiplx_html_7e32e4099349b84.png)
(Picture to be added here - docs work in progress)

Once connected, you'll need to open your web browser and connect to the captive portal which will allow you to configure your Wi-Fi connection and other parameters.

![](RackMultipart20221224-1-9tiplx_html_414bc12dc92d274c.png)
(Picture to be added here - docs work in progress)

Once opened, you should see this webpage, click on 'Configure WiFi'.

![](RackMultipart20221224-1-9tiplx_html_32c207bd5b8f25dc.png)
(Picture to be added here - docs work in progress)

Once you're on the WiFi configuration page, you'll have various options to set – such as the WiFi network you'd like the MicroFruit use to get weather and time updates, the password for that network, language, geographic location, and time zone information.

**Note: Your language, city for weather, weather API token, and time zone will be set based on your shipping address. You can change these to something else if you'd like, see the next section of this guide to learn how to do that, but if you're happy with your current address – don't change these settings.**

**For now, let's just set up our WiFi network. Click the WiFi network you want to connect to, in our case this will be 'Wifi Connection', and then fill in the password. Once complete, click 'Save'.**

![](RackMultipart20221224-1-9tiplx_html_a1a4420e30129fd2.png)
(Picture to be added here - docs work in progress)
**Once saved, you should see the following message.**

![](RackMultipart20221224-1-9tiplx_html_40ab9413a11b10f4.png)
(Picture to be added here - docs work in progress)
**It should at this time, take a few minutes for your MicroFruit to connect to WiFi and then you should be in business. You'll now get a slide show of current weather, weather forecasts, and time/date. Enjoy your new little desk mate.**  **😊**

# To reset settings

**If you want to change the city, timezone, WiFi settings or anything else you'll need to reset the configuration. This is super easy to do and you can accomplish this by sliding the bottom plate of the MicroFruit back to expose the reset button like this:**

**To reset, press the reset button once, wait until the "Hello" screen pops up, and press it once more.**  **Do not press it more than two times.** Once the "Hello" screen is displayed, you can connect into the WiFi hotspot and then make any changes you might need – the device will save and display your previous settings with the exception of your WiFi connection information.

![](RackMultipart20221224-1-9tiplx_html_a1a4420e30129fd2.png)
(Picture to be added here - docs work in progress)
# Change the City

**Like with any changes, if your settings are already configured you'll want to reset the MicroFruit using the 'reset settings' instructions. MicroFruit uses the OpenWeatherAPI to provide weather information. You'll need to locate your new City code from the OpenWeatherMap website. To do this:**

1. **Go to https://openweathermap.org/find?q= and search for a location.**

![](RackMultipart20221224-1-9tiplx_html_c318bc0a6aae4856.png)
(Picture to be added here - docs work in progress)
1. **Go through the result set and select the entry closest to the actual location you want to display data for.**

![](RackMultipart20221224-1-9tiplx_html_10e0ddcc19e36fbf.png)
(Picture to be added here - docs work in progress)
1. **Look in the URL of the browser – note the number in URL https://openweathermap.org/city/**** 2657896 ****. That number is the city code you'll need to add to the following field:**

![](RackMultipart20221224-1-9tiplx_html_3b3c731e2664ce61.png)
(Picture to be added here - docs work in progress)
# Change the API Key

If for whatever reason you need to configure a new API key for MicroFruit, you can do so by signing up for one. Here's how you do this:

1. Go to the signup page and sign up for a new OpenWeatherMap membership (it's free) [https://home.openweathermap.org/users/sign\_up](https://home.openweathermap.org/users/sign_up)

![](RackMultipart20221224-1-9tiplx_html_d99b9c41c26a147a.png)
(Picture to be added here - docs work in progress)

Once you've created and activated your account, you can now open the "API Keys" menu option on the OpenWeatherMap member portal.

![](RackMultipart20221224-1-9tiplx_html_edda2f39c879fdb1.png)
(Picture to be added here - docs work in progress)

To create a key, just type in the name of a key you'd like to generate, in our case let's use "MicroFruit" ![](RackMultipart20221224-1-9tiplx_html_652e7cfcfe3d4c2.png)

You'll then see a new API key appear. You'll need to copy and use the 'Key' value. Note – this is an example key only, and does not work.

![](RackMultipart20221224-1-9tiplx_html_35ce332a80312adc.png)
(Picture to be added here - docs work in progress)

# Change time zone

You can change the timezone, but it uses the POSTIX format to determine which timezone you'll be using from the network time servers. There are 461 mappings which are documented here, look up the closest city/time zone from the following location:

[https://github.com/nayarsystems/posix\_tz\_db/blob/master/zones.csv](https://github.com/nayarsystems/posix_tz_db/blob/master/zones.csv)

In column one, there's the name of the time zone, and in column two, there's the code which is used for the time zone. If for example you wanted to set your time zone to EST or New York time, you'd find New York in the list, and copy the code in column two and paste that into the timezone field in the MicroFruit settings.

![](RackMultipart20221224-1-9tiplx_html_a9104d84f06d6f2a.png)
(Picture to be added here - docs work in progress)
![](RackMultipart20221224-1-9tiplx_html_971a5b541e68e162.png)
(Picture to be added here - docs work in progress)

For common times in America, we've listed them in the application, but for the full list, you'll need to reference the mappings in the link above.
