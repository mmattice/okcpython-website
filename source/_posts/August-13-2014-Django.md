layout: post
title: "August 13 2014: Django"
tags: [Parallel Processing, Threading]
post_asset_folder: true
categories: [Meeting]
date: 2014-09-03 17:37:00
---



# Intro to Django

Monday
###August 13 2014
####6:30pm
####@Prototek

##About
Our Speaker this month is Buddy Lindsey Jr. who is going to give us an introduction to Django.  Django is a high-level Python Web framework that encourages rapid development and clean, pragmatic design.
<!-- more -->

##Speaker  

### Buddy Lindsey
##### [buddylindsey.com](http://buddylindsey.com/)
<div class="speaker-bio">
{% img speaker-headshot /images/speakers/buddy_lindsey.png  "Buddy Lindsey" "Buddy Lindsey" %}
Buddy Lindsey is a mostly self taught programmer and sometimes designer. He runs GoDjango.com which teaches beginner to advance Django topics.  He loves Django and has been working with it for 3 years. He also runs buddylindsey.com, a programming blog, consumeraffairs.com, and is an Eagle Scout, Husband, and Youth Pastor. 
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