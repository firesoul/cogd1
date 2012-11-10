<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
            "http://www.w3.org/TR/html4/strict.dtd">
<html>
<!--
Copyright 2010 by Dan Fabulich.

Dan Fabulich licenses this file to you under the
ChoiceScript License, Version 1.0 (the "License"); you may
not use this file except in compliance with the License. 
You may obtain a copy of the License at

 http://www.choiceofgames.com/LICENSE-1.0.txt

See the License for the specific language governing
permissions and limitations under the License.

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
either express or implied.
-->
<head>
<meta http-equiv="X-UA-Compatible" content="IE=7"/>
<meta name="viewport" content="width = device-width, initial-scale = 1.0, maximum-scale = 1.0">
<title>Multiple Choice Royal Navy Game | Choice of Broadsides</title>
<meta name="description" content="Multiple-choice swashbuckling naval adventure, in the spirit of C.S. Forester's Hornblower or Patrick O'Brian's Aubrey/Maturin books, with a dash of Jane Austen.">
<link rel="canonical" href="/broadsides/"/>
<script src="persist.js"></script>
<script src="util.js"></script>
<script src="ui.js"></script>
<script src="scene.js"></script>
<script src="navigator.js"></script>
<script>window.version="UNKNOWN"</script>
<script src="version.js"></script>
<script src="mygame.js"></script>
<link href="style.css" rel="stylesheet" type="text/css">
<script>if(window.isWebOS)document.write("<style>body {font-family: Prelude; font-size: 14pt}\n#header {font-size: 13pt}</style>");</script>
<link rel="icon" type="image/vnd.microsoft.icon" href="favicon.ico">
<meta name="apple-mobile-web-app-capable" content="yes"/>
<link rel="apple-touch-icon-precomposed" href="icons/mobile-icon.png"/>
<link rel="SHORTCUT ICON" href="favicon.ico"/>
<script>window.storeName="Broadsides";</script>
<script type="text/javascript">if(!isWeb&&window.isIosApp){document.write("<style>"+"#header { display: none; }"+""+"#emailUs { display: none; }"+""+"#main { padding-top: 1em; }"+"</style>"+"<meta name = 'viewport' content = 'width = "+window.innerWidth+"'>");window.addEventListener("resize",function(){document.querySelector("meta[name=viewport]").setAttribute("content","width="+window.innerWidth);var dummy=document.createElement("p");dummy.innerHTML="&nbsp;";document.body.appendChild(dummy);window.setTimeout(function(){document.body.removeChild(dummy)},10);},false);}
if(isWeb){document.write("<style>label:hover {background-color: rgba(153,136,119,0.2);}</style>");}
var rootDir="";</script>
</head>
<body>
<div id="advertisement">
</div>
<div id="header"><h1 class="gameTitle">Choice of Broadsides</h1>
<p>
<a href="credits.html" class="spacedLink">About</a>
<a href="http://www.choiceofgames.com/" onclick="moreGames(); return false;" class="spacedLink">More Games</a>
<a href="http://www.choiceofgames.com/blog" class="spacedLink">Blog</a>
<a href="javascript:subscribeLink();" class="spacedLink">Subscribe</a>
<span id="share"><span>Share on:</span>
<span><img height="16" width="16" src="icons/stumbleupon.png">
<a href="http://www.stumbleupon.com/submit?url=http%3A%2F%2Fwww.choiceofgames.com/broadsides/&amp;title=Choice+of+Broadsides" class="spacedLink">StumbleUpon</a></span>
<span><img height="16" width="16" src="icons/facebook.ico">
<a href="http://www.facebook.com/sharer.php?u=http://www.choiceofgames.com/broadsides/&amp;t=Multiple+Choice+Royal+Navy+Game+|+Choice+of+Broadsides" onclick="if (window.isFile) return true; window.open(&quot;http://www.facebook.com/sharer.php?u=http://www.choiceofgames.com/broadsides/&amp;t=Multiple+Choice+Royal+Navy+Game+|+Choice+of+Broadsides&quot;,&quot;sharer&quot;,&quot;toolbar=0,status=0,width=626,height=436&quot;);return false;" class="spacedLink">Facebook</a></span>
<span><img height="16" width="16" src="icons/twitter.ico">
<a href="https://twitter.com/intent/tweet?related=choiceofgames&amp;text=Awesome+game%3A+Choice+of+Broadsides&amp;url=http%3A%2F%2Fwww.choiceofgames.com/broadsides/&amp;via=choiceofgames" class="spacedLink">Twitter</a></span>
</span>
</p>
<p><button id="statsButton" onclick="showStats()">Show Stats</button></p>
</div>
<div id="main">
<div id="text">
<script>document.write('<div id="loading"><p>Loading...</p><p><img src=\"loader.gif\"></p></div>');</script>
</div>
</div>
<div id="mobileLinks" class="webOnly">
<p class="mobileBadges">
<a class='spacedLink' id='iphoneLink' href='http://itunes.apple.com/us/app/choice-of-broadsides/id365660770'><img src='icons/appstore.png' style='height: 3em;'></a>
<a class='spacedLink' id='androidLink' href='https://play.google.com/store/apps/details?id=com.choiceofgames.broadsides'><img src='icons/droid.png' style='height: 3em;'></a>
<a class='spacedLink' id='kindleLink' href='http://www.amazon.com/Choice-of-Broadsides/dp/B004FRH3PO'><img src='icons/kindle.png' style='height: 3em;'></a>
</p>
</div>
<p id="emailUs">Love it? Hate it? Write us at <a id="supportEmail" href='mailto:support-broadsides@choiceofgames.com'>support@choiceofgames.com</a></p>
<noscript>
<p>"Choice of Broadsides" is a multiple-choice swashbuckling naval adventure, in the spirit of C.S. Forester's Hornblower or Patrick O'Brian's Aubrey/Maturin books, with a dash of Jane Austen.</p>
<p>This game requires JavaScript; please enable JavaScript and refresh this page.</p>
<p>If you can't get the game to work, please write to us at <a href="mailto:support-broadsides@choiceofgames.com">support-broadsides@choiceofgames.com</a> for assistance.</p>
</noscript>
<script type="text/javascript">var _gaq=_gaq||[];_gaq.push(['_setAccount','UA-11851531-1']);_gaq.push(['_trackPageview']);if(isWeb){(function(){var ga=document.createElement('script');ga.type='text/javascript';ga.async=true;ga.src=('https:'==document.location.protocol?'https://ssl':'http://www')+'.google-analytics.com/ga.js';var s=document.getElementsByTagName('script')[0];s.parentNode.insertBefore(ga,s);})();}</script>
</body>
</html>
