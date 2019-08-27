# Pursuit-Core-Introduction-To-Networking-and-APIs-Lab

# Part One

Status Code Scavenger Hunt!

Use Postman to find each of the following HTTP codes:


For each of the questions below, write:

1. The the website which generated the HTTP status code
2. A description about what the status code means
3. If an app you were writing encountered this status code, what would you do (if anything) to resolve any issues?



For reference, see:

https://en.wikipedia.org/wiki/List_of_HTTP_status_codes (Links to an external site.)
https://http.cat

```swift
/*
1. 200 OK
    a. https://http.cat/
    b. the code means a successful request
    c. nothing needs to be done
    
2. 301 Moved Permanently
    a. hard to find one
    b. sends you to the new location of past address
    c. update to the new URL
    
3. 400 Bad Request
    a. https://httpstat.us/400
    b. Request cannot be fulfilled because of bad syntax
    c. correct the spelling/ syntax
    
4. 401 Unauthorized
    a. https://httpstat.us/401
    b. aunthentication failed wronf user/password
    c. remeber your login credentials somewhere
    
5. 403 Forbidden 
    a. https://api.nasa.gov/planetary/apod?api_key=QYzbmgCeWrSQxYaa49QFdlFb7a3S8U22zAlq8hvYs
    b. The server refused the authentication
    c. make sure the URL you typed in is correct
    
6. 404 Not Found
    a. https://dog.ceo/api/breed//image/random
    b. The resource could not be found
    c. The site may be private or it just doesn't exist so try something else
    
7. 418 I'm a teapot
    a. https://httpstat.us/418
    b. 1998 April fool joke
    c. short and stout, here is my handle, here is my spout
    
8. 500 Internal Server Error
    a. https://httpstat.us/500
    b. generic error message when no more specific message is suitable
    c.
*/
```

# Part Two

API Scavenger Hunt!

For each of the questions below, identify a website and search query that will give you the appropriate JSON.  Paste the url and the json below.  Googling the category + API will generally take you to where you need.  Ex. https://lmgtfy.com/?q=cat+fact+api

```swift
1. A random cat fact
https://catfact.ninja/breeds?limit=1
<details>
<summary>JSON code</summary>
"total": 98,
"per_page": "1",
"current_page": 1,
"last_page": 98,
"next_page_url": "https://catfact.ninja/breeds?page=2",
"prev_page_url": null,
"from": 1,
"to": 1,
"data": [
{
"breed": "Abyssinian",
"country": "Ethiopia",
"origin": "Natural/Standard",
"coat": "Short",
"pattern": "Ticked"
}
]
}
</details>

2. A list of 150 random users in English.
https://randomuser.me/
<details>
<summary> JSON code </summary>
<!DOCTYPE html><html lang="en"><head><title>Random User Generator | Home</title><meta charset='utf-8'><meta name="description" content="Random user generator is a FREE API for generating placeholder user information. Get profile photos, names, and more. It's like Lorem Ipsum, for people."><meta name="apple-mobile-web-app-capable" content="yes"><meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no"><link rel="stylesheet" type="text/css" href="dist/style.css"><script src="dist/all.js"></script></head><body class=""><div id="navbar" class=""><div class="nav_toggle"><div class="icon"><div></div><div></div><div></div></div></div><ul><li><a href="index">Home</a></li><li><a href="photos">User Photos</a></li><li><a href="documentation">Documentation</a></li><li><a href="changelog">Change Log</a></li><li><a href="stats">Stats &amp; Graphs</a></li><li><a href="donate">Donate</a></li><li><a href="copyright">Copyright Notice</a></li><li class="blank"></li><li><a href="photoshop">Photoshop Extension</a></li></ul></div><header><h1>Random User Generator</h1><p>A free, <a id="openSource" href="https://github.com/RandomAPI/Randomuser.me-Node">open-source</a> API for generating random user data. Like Lorem Ipsum, but for people. </p><a href="https://twitter.com/randomapi" class="twitter"><img src="img/twitter.png">Follow us @randomapi</a></header><div class="frame card_offset"><div class="card"><div class="details"><div class="user_photo horizontal_center" id="user_photo"><a href="javascript:getNewUser();" class="refresh">New</a><img src=""></div><p id="user_title">Hi, My name is</p><p id="user_value">...</p></div><ul class="values_list horizontal_center" id="values_list"><li data-title="Hi, My name is" data-value="..." data-label="name" class="active"></li><li data-title="My email address is" data-value="..." data-label="email" data-caps="false"></li><li data-title="My birthday is" data-value="..." data-label="birthday"></li><li data-title="My address is" data-value="..." data-label="location"></li><li data-title="My phone number is" data-value="..." data-label="phone"></li><li data-title="My password is" data-value="..." data-label="pass" data-caps="false"></li></ul></div><section class="sponsor"><h2>Sponsored</h2><h3>RandomAPI</h3><p>Want to create your own <b>customized</b> data generator for your application?<br>Check out our other service RandomAPI!</p><button id="learnmore" class="button" onClick="window.open('https://randomapi.com');">Learn More</button></section><section class="advertisement"><script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script><ins class="adsbygoogle" style="display:inline-block;width:230px;height:200px" data-ad-client="ca-pub-2036801804961954" data-ad-slot="7646598623"></ins><script>(adsbygoogle = window.adsbygoogle || []).push({});</script><ins class="adsbygoogle" style="display:inline-block;width:230px;height:200px;margin:0 16px;" data-ad-client="ca-pub-2036801804961954" data-ad-slot="7646598623"></ins><script>(adsbygoogle = window.adsbygoogle || []).push({});</script><ins class="adsbygoogle" style="display:inline-block;width:230px;height:200px" data-ad-client="ca-pub-2036801804961954" data-ad-slot="7646598623"></ins><script>(adsbygoogle = window.adsbygoogle || []).push({});</script></section><section><h2>How to use</h2><p>You can use AJAX to call the Random User Generator API and will receive a randomly generated user in return. If you are using jQuery, you can use the $.ajax() function in the code snippet below to get started.</p><pre>$.ajax({
url: '<span>https: //randomuser.me/api/</span>',
dataType: '<span>json</span>',
success: function(<span>data</span>) {
console.log(<span>data</span>);
}
});
</pre></section><section><h2>Results</h2><p>The application will provide you with a JSON, XML, CSV, or YAML object that you can parse and apply to your application.</p><p>You can specify the format you want the results in using the <a href="documentation#format">format</a> parameter.</p><pre>{
"results": [
{
"gender": "<span>male</span>",
"name": {
"title": "<span>mr</span>",
"first": "<span>rolf</span>",
"last": "<span>hegdal</span>"
},
"location": {
"street": "<span>ljan terrasse 346</span>",
"city": "<span>vear</span>",
"state": "<span>rogaland</span>",
"postcode": "<span>3095</span>",
"coordinates": {
"latitude": "<span>54.8646</span>",
"longitude": "<span>-97.3136</span>"
},
"timezone": {
"offset": "<span>-10:00</span>",
"description": "<span>Hawaii</span>"
}
},
"email": "<span><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="cdbfa2a1abe3a5a8aaa9aca18da8b5aca0bda1a8e3aea2a0">[email&#160;protected]</a></span>",
"login": {
"uuid": "<span>c4168eac-84b8-46ea-b735-c9da9bfb97fd</span>",
"username": "<span>bluefrog786</span>",
"password": "<span>ingrid</span>",
"salt": "<span>GtRFz4NE</span>",
"md5": "<span>5c581c5748fc8c35bd7f16eac9efbb55</span>",
"sha1": "<span>c3feb8887abed9ec1561b9aa2c9f58de21d1d3d9</span>",
"sha256": "<span>684c478a98b43f1ef1703b35b8bbf61b27dbc93d52acd515e141e97e04447712</span>"
},
"dob": {
"date": "<span>1975-11-12T06:34:44Z</span>",
"age": <span>42</span>
},
"registered": {
"date": <span>"2015-11-04T22:09:36Z</span>",
"age": <span>2</span>
},
"phone": "<span>66976498</span>",
"cell": "<span>40652479</span>",
"id": {
"name": "<span>FN</span>",
"value": "<span>12117533881</span>"
},
"picture": {
"large": "<span>https://randomuser.me/api/portraits/men/65.jpg</span>",
"medium": "<span>https://randomuser.me/api/portraits/med/men/65.jpg</span>",
"thumbnail": "<span>https://randomuser.me/api/portraits/thumb/men/65.jpg</span>"
},
"nat": "<span>NO</span>"
}
],
"info": {
"seed": "<span>2da87e9305069f1d</span>",
"results": <span>1</span>,
"page": <span>1</span>,
"version": "<span>1.2</span>"
}
}
</pre></section><section><h2>Thank you for helping us help you help us all</h2><p>Found a bug or have an idea?<br>Contribute to randomuser.me's database on our <a href="https://github.com/RandomAPI/Randomuser.me-Node">Github Repo</a>.</p><h2>Contact Us</h2><p>If you have any questions/feedback or would like to get in touch with us, tweet us <a href="https://twitter.com/randomapi">@randomapi</a></p></section><section class="cheat"><p>&uarr; &uarr; &darr; &darr; &larr; &rarr; &larr; &rarr; B A</p></section></div><footer><div class="frame"><h1>Random User Generator</h1><div class="block"><div class="builder"><h3>Designed</h3><a href="https://twitter.com/arronhunt"><img src="img/creator_arron.png" width="80px" alt="Designed by Arron Hunt" title="Designed by Arron Hunt" /></a></div><div class="builder"><h3>Developed</h3><a href="https://twitter.com/solewolf1993"><img src="img/creator_keith.png" width="80px" alt="Developed by Keith Armstrong" title="Developed by Keith Armstrong" /></a></div></div><div class="block"><h3>Copyright Notice</h3><p>All randomly generated photos were hand picked from the authorized section of <a href="http://uifaces.com">UI Faces</a>. Please visit <a href="https://web.archive.org/web/20160811185628/http://uifaces.com/faq">UI Faces FAQ</a> for more information regarding how you can use these faces.<br><br></div></div></footer><script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script>(function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject'
]=r;i[r
]=i[r
]||function(){(i[r
].q=i[r
].q||[]).push(arguments)
},i[r
].l=1*new Date();a=s.createElement(o),m=s.getElementsByTagName(o)[
0
];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
})(window,document,'script',' //www.google-analytics.com/analytics.js','ga');ga('create', 'UA-42942064-1', 'randomuser.me');ga('send', 'pageview');</script></body></html>
</details>


3. The current stock price of Microsoft. (IEX API)
https://ws-api.iextrading.com/1.0/tops
<details>
<summary> JSON code </summary>
{
"symbol": "IEX",
"sector": "capitalgoods",
"securityType": "commonstock",
"bidPrice": 160.3,
"bidSize": 100,
"askPrice": 0,
"askSize": 0,
"lastUpdated": 1566844702443,
"lastSalePrice": 160.6,
"lastSaleSize": 15,
"lastSaleTime": 1566844417050,
"volume": 7580,
"marketPercent": 0.03472
}
</details>


4. The 5 year history of Apple stock prices (IEX API)
<details>
https://ws-api.iextrading.com/1.0/tops
<summary> JSON code </summary>
{
"symbol": "AAPL",
"sector": "technologyhardwareequipment",
"securityType": "commonstock",
"bidPrice": 205.63,
"bidSize": 100,
"askPrice": 205.84,
"askSize": 100,
"lastUpdated": 1566844702555,
"lastSalePrice": 205.76,
"lastSaleSize": 100,
"lastSaleTime": 1566844701988,
"volume": 488307,
"marketPercent": 0.02536
}
</details>

5. All the Swift language repos on Github with Pursuit in their name
<details>
https://github.com/joinpursuit/:org/repos
<summary> JSON code </summary>
Gave me 404 error no access rights maybe
</details>

6. A list of all Pokemon
<details>
https://pokeapi.co/api/v2/pokemon/bulbasaur/
<summary> JSON code </summary>
"abilities": [
{
"ability": {
"name": "chlorophyll",
"url": "https://pokeapi.co/api/v2/ability/34/"
},
"is_hidden": true,
"slot": 3
},
{
"ability": {
"name": "overgrow",
"url": "https://pokeapi.co/api/v2/ability/65/"
},
"is_hidden": false,
"slot": 1
}
],
"base_experience": 64,
"forms": [
{
"name": "bulbasaur",
"url": "https://pokeapi.co/api/v2/pokemon-form/1/"
}
</details>

7. A list of all items in Fortnite
<details>
https://fortnite-api.theapinetwork.com/store/get
require authentication token
<summary> JSON code </summary>
{
"success": false,
"error": "Please add your Authorization token.",
"eCode": "authorization.empty",
"_console": "https://console.fortniteapi.com"
}
</details>

8. A list of all Game of Thrones Episodes.
<details>
https://got-quotes.herokuapp.com/quotes
<summary> JSON code </summary>
{
"quote": "The fisherman drowned, but his daughter got Stark to the Sisters before the boat went down. They say he left her with a bag of silver and a bastard in her belly. Jon Snow, she named him, after Arryn.",
"character": "Davos"
}
</details>

9. A list of all songs with "Love" in the title.
<details>
https://github.com/XDeric/SongsSearchBar/blob/master/SongsTableViewSearchBar/Song.swift
<summary> JSON code </summary>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<link rel="dns-prefetch" href="https://github.githubassets.com">
<link rel="dns-prefetch" href="https://avatars0.githubusercontent.com">
<link rel="dns-prefetch" href="https://avatars1.githubusercontent.com">
<link rel="dns-prefetch" href="https://avatars2.githubusercontent.com">
<link rel="dns-prefetch" href="https://avatars3.githubusercontent.com">
<link rel="dns-prefetch" href="https://github-cloud.s3.amazonaws.com">
<link rel="dns-prefetch" href="https://user-images.githubusercontent.com/">



<link crossorigin="anonymous" media="all" integrity="sha512-UDS3MR1FfvqHmqZAs2MWSDCWPwLemVRLqCwld4/zfwH0vhv7I6RYmDnMnNAVQKP1YYvqnccOCH4iOhFaUUyrjw==" rel="stylesheet" href="https://github.githubassets.com/assets/frameworks-2e9090135c22aad5f56c2f72dcba7880.css" />
<link crossorigin="anonymous" media="all" integrity="sha512-l4JpykYR1c86XfE0TExTqRFbnoD7WA39FhTTEgPt22zLFiepYq+L+3XUGBZoGsnBv15oKHTomwpEAUrCbmoRqw==" rel="stylesheet" href="https://github.githubassets.com/assets/site-2f0f446a127a5a480dfb139991acd1cd.css" />
<link crossorigin="anonymous" media="all" integrity="sha512-ip0PbDWWMX/xpzE2prEhR95RqVx8aDPUKvBEz691/7Isc3uapauorbb1zFXT2I5Go5BTzaev9qh/wKMj9pH95A==" rel="stylesheet" href="https://github.githubassets.com/assets/github-cbb49d8cd46cbc8c522a95d52b21ab53.css" />





<meta name="viewport" content="width=device-width">

<title>SongsSearchBar/Song.swift at master · XDeric/SongsSearchBar · GitHub</title>
<meta name="description" content="Contribute to XDeric/SongsSearchBar development by creating an account on GitHub.">
<link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub">
<link rel="fluid-icon" href="https://github.com/fluidicon.png" title="GitHub">
<meta property="fb:app_id" content="1401488693436528">

<meta name="twitter:image:src" content="https://avatars1.githubusercontent.com/u/19171748?s=400&amp;v=4" /><meta name="twitter:site" content="@github" /><meta name="twitter:card" content="summary" /><meta name="twitter:title" content="XDeric/SongsSearchBar" /><meta name="twitter:description" content="Contribute to XDeric/SongsSearchBar development by creating an account on GitHub." />
<meta property="og:image" content="https://avatars1.githubusercontent.com/u/19171748?s=400&amp;v=4" /><meta property="og:site_name" content="GitHub" /><meta property="og:type" content="object" /><meta property="og:title" content="XDeric/SongsSearchBar" /><meta property="og:url" content="https://github.com/XDeric/SongsSearchBar" /><meta property="og:description" content="Contribute to XDeric/SongsSearchBar development by creating an account on GitHub." />

<link rel="assets" href="https://github.githubassets.com/">

<meta name="pjax-timeout" content="1000">

<meta name="request-id" content="61E3:37F9:E722D:130C94:5D643342" data-pjax-transient>




<meta name="selected-link" value="repo_source" data-pjax-transient>

<meta name="google-site-verification" content="KT5gs8h0wvaagLKAVWq8bbeNwnZZK1r1XQysX3xurLU">
<meta name="google-site-verification" content="ZzhVyEFwb7w3e0-uOTltm8Jsck2F5StVihD0exw2fsA">
<meta name="google-site-verification" content="GXs5KoUUkNCoaAZn7wPN-t01Pywp9M3sEjnt_3_ZWPc">

<meta name="octolytics-host" content="collector.githubapp.com" /><meta name="octolytics-app-id" content="github" /><meta name="octolytics-event-url" content="https://collector.githubapp.com/github-external/browser_event" /><meta name="octolytics-dimension-request_id" content="61E3:37F9:E722D:130C94:5D643342" /><meta name="octolytics-dimension-region_edge" content="iad" /><meta name="octolytics-dimension-region_render" content="iad" /><meta name="octolytics-dimension-ga_id" content="" class="js-octo-ga-id" /><meta name="octolytics-dimension-visitor_id" content="1176347009425354825" />
<meta name="analytics-location" content="/&lt;user-name&gt;/&lt;repo-name&gt;/blob/show" data-pjax-transient="true" />



<meta name="google-analytics" content="UA-3769691-2">


<meta class="js-ga-set" name="dimension1" content="Logged Out">
</details>

10. All information about Petyr Baelish from the Game of Thrones books
<details>
https://gameofthrones.fandom.com/wiki/Petyr_Baelish
<summary> JSON code </summary>
<!doctype html>
<html lang="en" dir="ltr" class="">
<head>

<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta name="viewport" content="width=device-width, user-scalable=yes">
<meta name="generator" content="MediaWiki 1.19.24" />
<meta name="keywords" content="Game of Thrones Wiki,gameofthrones,Petyr Baelish,Season 1,Season 2,Season 3,Season 4,Season 5,Season 6,Season 7,Lord Snow,The Dragon and the Wolf,Robert's Rebellion (Histories &amp; Lore)" />
<meta name="description" content="Lord Petyr Baelish, popularly called Littlefinger, was the Master of Coin on the small council under King Robert Baratheon and King Joffrey Baratheon. He was a skilled manipulator and used his ownership of brothels in King's Landing to both accrue intelligence on political rivals and acquire..." />
<meta name="twitter:card" content="summary" />
<meta name="twitter:site" content="@getfandom" />
<meta name="twitter:url" content="https://gameofthrones.fandom.com/wiki/Petyr_Baelish" />
<meta name="twitter:title" content="Petyr Baelish | Game of Thrones Wiki | FANDOM powered by Wikia" />
<meta name="twitter:description" content="Lord Petyr Baelish, popularly called Littlefinger, was the Master of Coin on the small council under King Robert Baratheon and King Joffrey Baratheon. He was a skilled manipulator and used his..." />
<link rel="canonical" href="https://gameofthrones.fandom.com/wiki/Petyr_Baelish" />
<link rel="apple-touch-icon" href="https://slot1-images.wikia.nocookie.net/__cb1565980047504/common/skins/common/images/wiki.png" sizes="155x155" />
<link rel="shortcut icon" href="https://slot1-images.wikia.nocookie.net/__cb1565980047504/common/skins/common/images/favicon.ico" />
<link rel="search" type="application/opensearchdescription+xml" href="/opensearch_desc.php" title="Game of Thrones Wiki (en)" />
<link rel="EditURI" type="application/rsd+xml" href="https://gameofthrones.fandom.com/api.php?action=rsd" />
<link rel="copyright" href="https://www.fandom.com/licensing" />
<link rel="alternate" type="application/atom+xml" title="Game of Thrones Wiki Atom feed" href="/wiki/Special:RecentChanges?feed=atom" />
<title>Petyr Baelish | Game of Thrones Wiki | FANDOM powered by Wikia</title>

<!-- CSS injected by skin and extensions -->
<link rel="stylesheet" href="https://slot1-images.wikia.nocookie.net/__am/1565980047504/sasses/background-dynamic%3Dtrue%26background-image%3Dhttps%253A%252F%252Fimg4.wikia.nocookie.net%252F__cb20150716154804%252Fgameofthrones%252Fimages%252F5%252F50%252FWiki-background%26background-image-height%3D720%26background-image-width%3D1920%26color-body%3D%2523000%26color-body-middle%3D%2523000000%26color-buttons%3D%25231e5467%26color-community-header%3D%25231e5467%26color-header%3D%25235f4416%26color-links%3D%252347518e%26color-page%3D%2523d7cbab%26oasisTypography%3D1%26page-opacity%3D100%26widthType%3D0/skins/oasis/css/oasis.scss,extensions/wikia/Forum/css/ForumTag.scss,extensions/wikia/DesignSystem/styles/design-system.scss,extensions/wikia/CommunityHeader/styles/index.scss,extensions/wikia/PageHeader/styles/index.scss,extensions/wikia/Recirculation/styles/recirculation.scss,extensions/wikia/EmbeddableDiscussions/styles/EmbeddableDiscussions.scss,extensions/wikia/PortableInfobox/styles/PortableInfobox.scss,extensions/wikia/ArticleVideo/styles/jwplayer.scss,extensions/wikia/ArticleVideo/styles/jwplayer-overrides.scss,extensions/wikia/ArticleVideo/styles/video-feedback.scss,extensions/wikia/ArticleVideo/styles/video-attribution.scss,extensions/wikia/AdEngine3/dist/styles.scss,extensions/wikia/Qualaroo/css/Qualaroo.scss" /><link rel="stylesheet" href="/load.php?cb=1565980047504&debug=false&lang=en&modules=site&only=styles&skin=oasis&*" /><style>a:lang(ar),a:lang(ckb),a:lang(fa),a:lang(kk-arab),a:lang(mzn),a:lang(ps),a:lang(ur){text-decoration:none
}a.new,#quickbar a.new{color:#ba0000
}
/* cache key: gameofthrones:resourceloader:filter:minify-css:7:c88e2bcd56513749bec09a7e29cb3ffa */</style>


<script>
var Wikia={},
wgUseSiteJs=true,
wgWikiVertical="tv",
wgWikiCategories=[],
wgMessages={
"categoryselect-button-save": "Save",
"categoryselect-category-add": "Add category...",
"categoryselect-category-edit": "Edit category",
"categoryselect-category-remove": "Remove category",
"categoryselect-error-category-name-length": "The maximum length for a category name has been reached.",
"categoryselect-error-duplicate-category-name": "Category \"$1\" already exists.",
"categoryselect-error-empty-category-name": "Please provide a category name.",
"categoryselect-modal-category-name": "Provide the name of the category:",
"categoryselect-modal-category-sortkey": "Optionally, you may alphabetize this page on the \"$1\" category page under the name:",
"categoryselect-tooltip-add": "Press the Enter or Return key when done."
},
wgOnSiteNotificationsApiUrl="https://services.fandom.com/on-site-notifications",
JSSnippetsStack=[],
ads={
"context": {
"bidders": [],
"opts": {
"adsInContent": 1,
"enableCheshireCat": true,
"pageType": "all_ads",
"showAds": true
},
"targeting": {
"enableKruxTargeting": true,
"enablePageCategories": true,
"esrbRating": "mature",
"mappedVerticalName": "ent",
"pageArticleId": 2220,
"pageIsArticle": true,
"pageName": "Petyr_Baelish",
"pageType": "article",
"wikiCategory": "ent",
"wikiCustomKeyValues": "age=18-24;age=25-34;age=18-34;esrb=mature;gnre=action;gnre=adventure;gnre=drama;gnre=fantasy;gnre=fighting;media=tv;media=books;sex=f;sex=m;theme=dragon;theme=magic;theme=mature;theme=sword;theme=zombie;tv=hbo",
"wikiDbName": "gameofthrones",
"wikiId": "130814",
"wikiIsTop1000": true,
"wikiLanguage": "en",
"wikiVertical": "tv",
"newWikiCategories": [
"ent"
],
"hasPortableInfobox": true,
"hasFeaturedVideo": true,
"featuredVideo": {
"mediaId": "bdiBbuFp",
"videoTags": [
"TV",
"Game of Thrones",
"Featured Video",
"FV-Originals",
"EN",
"Voiceover",
"Dec-17"
]
}
}
},
"runtime": {
"disableBtf": false
}
}
</details>

11. All the movies Leonardo Dicaprio has acted in
<details>
https://en.wikipedia.org/wiki/Leonardo_DiCaprio_filmography
<summary> JSON code </summary>
<!DOCTYPE html>
<html class="client-nojs" lang="en" dir="ltr">
<head>
<meta charset="UTF-8"/>
<title>Leonardo DiCaprio filmography - Wikipedia</title>
<script>document.documentElement.className=document.documentElement.className.replace(/(^|\s)client-nojs(\s|$)/,
"$1client-js$2");RLCONF={
"wgCanonicalNamespace": "",
"wgCanonicalSpecialPageName":!1,
"wgNamespaceNumber": 0,
"wgPageName": "Leonardo_DiCaprio_filmography",
"wgTitle": "Leonardo DiCaprio filmography",
"wgCurRevisionId": 912032765,
"wgRevisionId": 912032765,
"wgArticleId": 35934168,
"wgIsArticle":!0,
"wgIsRedirect":!1,
"wgAction": "view",
"wgUserName": null,
"wgUserGroups": [
"*"
],
"wgCategories": [
"Use mdy dates from October 2015",
"Articles with hCards",
"Turner Classic Movies person ID not in Wikidata",
"Featured lists",
"Male actor filmographies",
"American filmographies",
"Leonardo DiCaprio"
],
"wgBreakFrames":!1,
"wgPageContentLanguage": "en",
"wgPageContentModel": "wikitext",
"wgSeparatorTransformTable": [
""
</details>

```
