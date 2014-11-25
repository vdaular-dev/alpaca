---
layout: page
title: Easy Forms for jQuery
title2: Alpaca - Easy Forms for jQuery
description: Easily create forms for your web site using Alpaca, jQuery and Bootstrap
keywords: alpaca,forms,jquery,bootstrap
#tagline: Easy Forms for jQuery
---
{% include JB/setup %}

Alpaca provides the easiest way to generate interactive HTML5 forms for web and mobile applications.
It uses JSON Schema and simple Handlebars templates to generate great looking user interfaces on top of
<a href="http://twitter.github.com/bootstrap" target="_blank">Twitter Bootstrap</a>,
<a href="http://jqueryui.com" target="_blank">jQuery UI</a>,
<a href="http://jquerymobile.com" target="_blank">jQuery Mobile</a>
and HTML5.

Everything you need is provided out of the box.  Alpaca comes pre-stocked with a large library of controls,
templates, layouts and features to make rendering JSON-driven forms easy.  It is designed around an extensible
object-oriented pattern, allowing you to implement new controls, templates, I18N bundles and custom data
persistence for your projects.

Alpaca is open-source and provided to you under the Apache 2.0 license.  It is supported by
<a href="https://www.cloudcms.com">Cloud CMS</a> and is in use by organizations and within projects all around the world.

<div class="video-container" align="center">
     <iframe src="http://www.youtube.com/embed/mK4BXiGNbvA" frameborder="0" width="560" height="315"> </iframe>
</div>


## How do I use Alpaca?

<!-- STEP 1 -->
<div class="step">
    <img src="{{ BASE_PATH }}/images/step-1.png"/>
    Copy the following into the <code>&lt;head/&gt;</code> block of your web page:
    <br/>
    <br/>

<div class="codewrap">
<pre class="prettyprint linenums">
&lt;script type="text/javascript" src="//code.cloudcms.com/alpaca/1.5.0/bootstrap/alpaca.min.js"&gt;&lt;/script&gt;
&lt;link type="text/css" href="//code.cloudcms.com/alpaca/1.5.0/bootstrap/alpaca.min.css" rel="stylesheet"/&gt;
</pre>
</div>

</div>

<!-- STEP 2 -->
<div class="step">
    <img src="{{ BASE_PATH }}/images/step-2.png"/>
    Call <code>$.alpaca()</code> with your form schema and any configuration:
    <br/>
    <br/>

<div class="codewrap">
<pre class="prettyprint linenums">
&lt;div id="form1"&gt;&lt;/div&gt;
&lt;script type="text/javascript"&gt;
$("#form1").alpaca({
    "schema": {
        "title": "What do you think of Alpaca?",
        "type": "object",
        "properties": {
            "name": {
                "type": "string",
                "title": "Name"
            },
            "ranking": {
                "type": "string",
                "title": "Ranking",
                "enum": ['excellent', 'not too shabby', 'alpaca built my hotrod']
            }
        }
    }
});
&lt;/script&gt;
</pre>
</div>

</div>

<!-- STEP 3 -->
<div class="step">
    <img src="{{ BASE_PATH }}/images/step-3.png"/>
    Enjoy your newly rendered Alpaca form!
    <br/>
    <br/>
    <div class="tutorial-panel">
        <div class="panel panel-default">
          <div class="panel-body">
            <div id="form1"></div>
          </div>
        </div>
    </div>
</div>


## Who uses Alpaca?

Lots of people.  Alpaca is an open-source project and has been around for almost 3 years.  We've had a great time
building it and have enjoyed the pull requests and adoption within some really great companies worldwide.  Here
are a few notable ones:

<div class="community">

    <div class="row">
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.pearsoned.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/pearson-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.fox.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/fox-entertainment-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.trinet.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/trinet-150.jpg" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.cloudcms.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/cloudcms-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
    </div>
    <div class="row">
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.sony.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/sony-150.jpg" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://hbsp.harvard.edu/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/harvard-business-publishing-150.jpg" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.biogenidec.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/biogen-idec-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.exari.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/exari-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
    </div>
    <div class="row">
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.virginmobileusa.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/virgin-mobile-150.jpg" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.sprint.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/sprint-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.evolvedmediasolutions.co.uk/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/evolved-media-solutions-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
        <div class="col-md-3">
            <div class="icon-holder">
                <a href="http://www.fxnetworks.com/" target="_blank">
                    <img src="{{ BASE_PATH }}/images/community/fx-networks-150.png" style="max-width:125px" />
                </a>
            </div>
        </div>
    </div>
</div>

If you'd like to have your company logo listed above, please <a href="support.html">drop us a line</a>.


## What Browsers are Supported?

Alpaca works in with any browser that supports jQuery 1.10.x and above.  This includes web browsers and
browsers running on mobile devices.

We've tested Alpaca against IE 9 and beyond.  It may work with earlier versions but you're getting into tedious
territory there.  This is not your fault.  Don't blame yourself.  Just be thorough and give your forms a test on IE 8
and below.


## Is Alpaca open source?

Yes.  Alpaca is an open-source project and the source code is freely available under the Apache 2 license.  We chose
the Apache 2 license because it is permissive and lets you get the most out of open source.

We any luck, Alpaca will improve your life.  Save you time.  And let you play with your kids more.

Alpaca is supported by the community and several active contributors who have supplied pull requests with new features,
ideas and technical wonder.  The project started at Cloud CMS where we used Alpaca as our forms engine of choice.

If you have a question or think that you've found a bug, please visit our
<a href="https://github.com/gitana/alpaca" target="_blank">GitHub Issues page</a> and let the community know.
 Chances are that someone has run into something similar and can help out.

You can freely <a href="https://github.com/gitana/alpaca" target="_blank">fork Alpaca</a> by visiting the
<a href="https://github.com/gitana/alpaca" target="_blank">Alpaca project at GitHub</a>.


## Is Alpaca supported?

Yes, Alpaca is supported if you <a href="support.html">sign up for a support contract with Cloud CMS</a>.
We have engineers who offer consulting services, technical support and training.

<a href="https://www.cloudcms.com" target="_blank">Cloud CMS</a> sponsors Alpaca and is ready to work with you to support your live engagements.

<a href="support.html">Let us know how we can help</a>!


## How do I get started?

You can drop Alpaca into your new or existing web or mobile projects.  Alpaca is a simple JavaScript library that
you can plug in wherever you'd like.  You can <a href="download.html">install or download Alpaca</a> using conventional
tools like Bower or NPM.  Or you can <a href="download.html">grab a release</a> from our
 <a href="download.html">download page</a>.

<script>
$("TABLE.stack").dataTable({
    "bAutoWidth": false,
    "bInfo": false,
    "bLengthChange": false,
    "bFilter": false,
    "bPaginate": false
});
</script>

<script>
$("#form1").alpaca({
    "schema": {
        "title": "What do you think of Alpaca?",
        "type": "object",
        "properties": {
            "name": {
                "type": "string",
                "title": "Name"
            },
            "ranking": {
                "type": "string",
                "title": "Ranking",
                "enum": ['excellent', 'not too shabby', 'alpaca built my hotrod']
            }
        }
    },
    "options": {
        "focus": false
    }
});
</script>