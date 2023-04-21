# Class 41 Reading

## What does Progressive in Progressive Web App mean?

This means that our platform specific apps(which usually feel as if they are apart of the machine they are working on) are working alongside "modern API's" this helps deliver the benefits of any platform specific app(These are often very reliable and can work with hardware attached via USB, can work even with weak connection, and can even use files stored on the users device) as well the capabilities and reliability and instabillity while having the reach that often comes with webapps.

## What are three benefits of writing a progressive web app, as opposed to a native app?

1.) We are able to increase the abilities that this app can do, this makes users feel much butter about the app because we are able top ensure that the app still does what it needs to at its core, 2.) this could really increase the amount of traffic and interation.

3.)This also helps the relaiabillity of the app (as stated above) we are able to make sure that the data that this app is used for is still accessible to the user, this could be very important especially if the user uses this app for work or anything that their livihood relys on.

## What are two reasons to consider a native app, instead of a PWA?

I think if connection was a big reason for an app (instead of interactivity like widgets). Then assuring the user has the constant reliablility for this app is a big deal.

I also think that maybe this app is just something that requires no one to interact with constantly, other than a simple "check-in".

## When a website has an app manifest, what is it able to do?

The App Manifest is kind of the like the `README` of your webapp. This is a JSON file that tells the browser things like the name of your app, how it is supposed to behave when it is installed and even the icons needed for the app itself as well as the URL that should be launched when you open/ use the app.

## Name and describe how short_name and two other manifest properties are used

`short_name` is kind of like the apps first name, its the simplest name needed to still understand your apps name and what it does. It is also the name that is used on the user homescreen.

`name` is used when the app is installed. This is the "full" name of the app.

`icons` is an array of image objects which also has the `src` `sizes` and `type` properties.

`start_url` tells the browser where the user will start on when they start up your app. This is really helpful especially when the user was using the app before, this makes sure that you have a "home screen". "think about what the user will want once they open your app, and place them there" 

## How does Chrome render a PWA splash screen?

Chrome pulls from the manifest properties (`name` `background_color` and `icons`) to fill out your screen as its loading. This shows the user that everything is working and being loaded as expected, it just may take a second to get everything painted on the screen.
