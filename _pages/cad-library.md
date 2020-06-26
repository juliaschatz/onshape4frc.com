---
layout: page
title: CAD Library
permalink: /cad-library
comments: false
---

<div class="row justify-content-between">
<div class="col-md-8 pr-5">

<p>One of the great things about Onshape are the parts libraries and featurescripts created by the community. This page is a list of some of the most useful ones we've found.</p>

<div id="MKCad">
<h4>MKCad Onshape Library</h4>

<p>This library has a wide variety of COTs parts which can be easily imported into your assemblies. This is a community created library and you can see its latest updates in the <a target="_blank" href="https://www.chiefdelphi.com/t/mkcad-2020-season-updates/367821">ChiefDelphi Thread</a>. You can find the different documents by searching for them in the public section of onshape or simply clicking <a target="_blank" rel="noopener noreferrer" href="https://cad.onshape.com/documents?nodeId=3&resourceType=filter&q=_all:MKCad">this link</a>.</p>

<p>To easily find these documents when it is time to insert them into your assemblies it is recommended to tag them. This process is outlined in our <a href="/getting-started#mkcad">getting started page</a>.</p>

</div>

<div id="Featurescripts">
<h4>Featurescripts</h4>

<p>Onshape has their own scripting language to create custom features to automate aspects of design called <a target="_blank" href="https://www.onshape.com/features/custom-features">Featurescripts</a>. There are also a lot of community generated scripts which are particularly useful to FRC.</p>

<p>
  <button class="btn btn-primary" type="button" data-toggle="collapse" data-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
    Learn how to install Featurescripts &raquo;
  </button>
</p>
<div class="collapse" id="collapseExample">
  <div class="card card-body">
    <ol>
        <li>Open any Onshape document</li>
        <li>Click the right most button on the toolbar ('Add custom features')</li>
        <li>Paste the link of the Featurescript you're looking to add into the search bar (you can use the 'Copy Link' button next to the below scripts')
        <ul>
            <li>Note: Many of the below feature scripts are part of the same overall document so you can add multiple from the same link.</li>
        </ul>
        </li>
        <li>Select the given script you want. It is then accessible from the same drop down where you added the feature.</li>
    </ol>
  </div>
</div>

{% for featurescript in site.featurescripts %}
{% assign feature = featurescript[1] %}

<h5>{{ feature.name }}</h5>

<div class="row">
    <div class="col-md-4 pr-5">
        <img class="img-fluid lazyimg" src="{{ feature.image }}">
    </div>
    <div class="col-md-8 pr-5">
    <p>{{ feature.description }}</p>
    <a target="_blank" rel="noopener noreferrer" 
    href="{{ feature.link }}">
    {{ feature.name }} Link
    </a>
    <a onClick="CopyText('{{ feature.link }}');" class="btn btn-secondary">Copy Link</a>
    </div>
</div>
<br>
{% endfor %}

</div>

</div>

<!-- Right side -->
<div class="col-md-4">

<div class="sticky-top sticky-top-80">
<h5>Are We Missing Anything?</h5>

<p>If we're missing any useful resources be sure to let us know so we can get it added.</p>

<a href="/contribute" class="btn btn-primary">Add to the CAD Library</a>

</div>
</div>
</div>

<script>
    function CopyText(text){
        // var text = "Example text to appear on clipboard";
        navigator.clipboard.writeText(text).then(function() {
            // console.log('Async: Copying to clipboard was successful!');
        }, function(err) {
            console.error('Async: Could not copy text: ', err);
        });
    }
</script>
