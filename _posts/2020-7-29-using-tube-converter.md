---
layout: post
title: "Using the TubeConverter Featurescript"
author: max
categories: [Onshape, Featurescripts]
image: assets/images/blog/tubes.png
featured: true
hidden: false
comments: false
---

This blog will walk you though using one of the most powerful featurescripts, the TubeConverter. This script is a real game changer for how quickly you can design parts, especially if you use a common hole pattern on your box tubing. Simply extrude the outer dimensions of your tube then use this script to shell out the internals and add in any common hole patterns.

There are configurations for many important parameters like wall thickness and what kind of hole pattern you want. There are a few major types of hole pattern which are named for either the VexPro versaframe system or patterns used by teams. Two examples of slightly different patterns are shown below. Each one also has the option to add in a center row of holes.

<div class="row justify-content-center">
    <div class="col-md-5 pr-5">
        <h5 class="text-center">1678 Pattern</h5>
        <img src="/assets/images/blog/TubeConverter1678.png" />
    </div>
    <div class="col-md-5 pr-5">
        <h5 class="text-center">4414/1323/973 Pattern</h5>
        <img src="/assets/images/blog/TubeConverter4414.png" />
    </div>
</div>

The user can also configure the hole size and offsets from one of the sides if you don't want it to be centered by default. It is also possible to exclude certain faces from the hole pattern if needed.

This featurescript has the possibility to speed up your workflow significantly if used right. It is also nice as it combines many operations into one feature to keep your feature bar clear and easier to see when you have to come back to modify something. This workflow is most powerful when you use a standardized build system with a precut pattern across most of your parts.

Shout out to <a href="https://www.chiefdelphi.com/u/dydx" target="_blank">Julia</a> on ChiefDelphi for sharing this (and many more) featurescript.
