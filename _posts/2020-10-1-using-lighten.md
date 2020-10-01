---
layout: post
title: "Using the Lighten Featurescript"
author: jack
categories: [Onshape, Featurescripts]
image: assets/images/blog/lighten/lighten-title.png
featured: true
hidden: false
comments: false
---

The lighten script is yet another powerful tool you can use to cut down on the time spent per part. Additionally, it drastically reduces the amount of manual work required to nicely lighten/pocket a part. 

Simply create a new sketch on a part, connect your load points with lines, and then use this script on the resulting sketch regions. Set your tool radius, wall thickness, and cut depth, and it pockets it for you!

<div class="row justify-content-center pb-4">
    <div class="col-md-10 pr-10">
        <h5 class="text-center">Lightening a Plate</h5>
        <img src="/assets/images/blog/lighten/lighten-fs-plate.png" />
    </div>
</div>

I find that having the ``Trim faces with part`` option selected usually results in more desirable pocketing, though it is often a case-by-case basis. If you run into issues with this script breaking after a change, or the script not liking your selections, I recommend removing your ``Faces to remove`` selections using the ``x`` and then reselecting the faces. Sometimes you’re able to notice which sketch region is breaking the script, and other times it seems to fix itself.

This featurescript has the possibility to dramatically speed up your workflow if used appropriately[^1]. The way the script is set up makes it super easy to quickly change the thickness of your walls or radius of your tool if later deemed necessary.

Shout out to <a href="https://www.chiefdelphi.com/u/dydx" target="_blank">Julia</a> on ChiefDelphi for sharing this (and many more) featurescript.

[^1]: Despite this script doing most of the work for you, you still need to know how your part interacts with forces around it. Simply using this script and hoping it doesn’t over-lighten it is not a good mindset to have.
