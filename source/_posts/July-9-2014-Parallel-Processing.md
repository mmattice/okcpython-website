layout: post
title: "July 9 2014: Parallel Processing in Python"
tags: [Parallel Processing, Threading]
post_asset_folder: true
categories: [Meeting]
date: 2014-09-03 17:37:00
---



# Weaving Your Fate

Monday
###July 9, 2014
####11:30 a.m.
####@Prototek

##About
We’ll be talking about some of the ways you can do parallel processing in Python. We’ll cover the threading package, the multiprocessing package, and directly interacting with the lower level system methods like os.fork and os.exec. You’ll walk away knowing what the heck GIL stands for, and some ways to do parallel processing in Python. Assuming you can thwart your destiny and throw off the shackles of single-threaded applications.

<!-- more -->

##Speaker  

### Alex Ward
#### [alextheward.com](https://alextheward.com/)
#### [@cthos](https://twitter.com/cthos )
<div class="speaker-bio">
{% img speaker-headshot /images/speakers/alex_ward.png  "Alex Ward" "Alex Ward" %}
Alex is a web developer in Oklahoma City working on a wide range of projects. He specializes in the full LAMP stack and is proficient in Python, Ruby, Java (Android), ActionScript 3 and C. He has worked on a wide variety of projects including Wizards of the Coast Community site, THQ, SoundManager, XMPP chat systems, Drupal 6 and 7 installs, MediaWiki installs and other web technologies. Presently he works for Acquia as a Migration Consultant.
</div>

##Prototek
Prototek
401 NW 10th,
Oklahoma City, Oklahoma
73101

<script 
type="text/javascript" 
src="http://maps.google.com/maps/api/js?sensor=false"
></script>
<style>
#gmap_canvas img{
  max-width:none!important;
  background:none!important;
}

.speaker-headshot {
  float: left;
  padding: 5px 15px 5px 0px; 
}

</style>

<div style="overflow:hidden;height:200px; max-width:940px;">
  <div id="gmap_canvas" style="height:200px; max-width:940px;"></div>
</div>
<script type="text/javascript"> 
function init_map() {
    var myOptions = {
        zoom: 14,
        center: new google.maps.LatLng(35.478527, -97.51941699999998),
        mapTypeId: google.maps.MapTypeId.ROADMAP
    };
    map = new google.maps.Map(document.getElementById("gmap_canvas"), myOptions);
    marker = new google.maps.Marker({
        map: map,
        position: new google.maps.LatLng(35.478527, -97.51941699999998)
    });
    infowindow = new google.maps.InfoWindow({
        content: "<b>Prototek</b><br/>401 NW 10th St, <br/>73103 Oklahoma City"
    });
    google.maps.event.addListener(marker, "click", function() {
        infowindow.open(map, marker);
    });
    infowindow.open(map, marker);
}
google.maps.event.addDomListener(window, 'load', init_map);
</script>