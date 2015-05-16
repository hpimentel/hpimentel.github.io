---
layout: post
title: Devoted for Android 
---

*Devoted* is an app for Android that takes and displays an RSS feed that gets updated daily. The app allows users to check for new devotionals every day and also to read all previous devotionals available. The user can share their favorite devotionals and subscribe to a different list of topics.

This app was developed from August to November 2014 during my internship at CIRC. Dr. Hall, my boss, gave me the app's requirements and then he took off my chains of dependability towards existing code bases. I was set free to code and come up with a product that resemble the ideas portrayed by our customers. 

Startin a project is always difficult; in this case it was difficult since it was my first time using **Android Studio** instead of **Eclipse**, and alsomy first time starting an app from scratch during my internship.

I can list all the things I learned in this project, but the most important where: how to fetch and parse an RSS feed in the background, how to deal with images in Android, and making sure the app worked in all supported Android devices.

One of the features of the app is that it caches previously seen devotionals, including its corresponding image. I quickly realize that caching and displaying images for all devices was going to be a difficult task. And then came [Picasso](http://square.github.io/picasso/) by Square. With a couple one liners I was able to do everything I wanted to do initally.

Another problem was having text wrapping around an image, which surprisingly Android does not support. After hours of trying things and searching on StackOverflow, I was able to find a library that along with a quick fix that conveyed converting pixel size to sp, fixed my problem (You can see more about this problem [here](http://stackoverflow.com/questions/26111609/android-text-around-image-bug/26183259#26183259) and visualize it below).

![Devoted bug]({{ site.url }}/images/2015-3-22/devotedProblem.jpg)

The app is out and you can download it in the [Play Store](https://play.google.com/store/apps/details?id=edu.southern.cs.circ.devoted).

