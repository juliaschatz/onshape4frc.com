---
layout: post
title: "Using the Extrude Individual Featurescript"
author: jack
categories: [Onshape, Featurescripts]
image: assets/images/blog/extrude-individual/title-image3.png
featured: true
hidden: false
comments: false
---

Extrude Individual creates a new body for each selected section of a sketch, allowing the user to quickly create multiple parts in a single operation. This script is particularly useful if you need multiple tubes of the same height, like a drivetrain or elevator.

Simply create a sketch and use the script to select the desired unique sketch regions. A new part will be created for each selected section of the sketch.

<div class="row justify-content-center pb-4">
    <div class="col-md-10 pr-10">
        <h5 class="text-center">Creating 4 Tubes in 1 Feature</h5>
        <img src="/assets/images/blog/extrude-individual/extrude-individual-dt.png" />
    </div>
</div>

This featurescript has the potential to seriously speed up your workflow if used appropriately. Furthermore, it can vastly reduce the amount of features in your feature tree, making it easier to both navigate and to modify.

Shout out to <a href="https://www.chiefdelphi.com/u/dydx" target="_blank">Julia</a> on ChiefDelphi for sharing this (and many more) featurescript.
