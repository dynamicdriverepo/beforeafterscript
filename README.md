# Before and After image script #

*Description:*  Nothing ever stays the same, which is why we created this Before and After script to easily view an "after" version of any image as an overlay of the original one. It makes for a dramatic way of comparing two images and any subtle differences. A draggable handle bar lets the user decide how much of each image he/she wishes to view. The "before" and "after" slides can each contain not just a main image, but other HTML as well, such as a caption. Furthermore, the script can load another set of images on demand.

## Directions ##

*Step 1:* This script uses the following external files:

+ jQuery 1.7 or above (served via Google CDN)
+ ddbeforeandafter.css
+ ddbeforeandafter.js

*Step 2:* Add the below code to the HEAD section of your page:

	<link rel="stylesheet" href="ddbeforeandafter.css" />
	
	<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
	
	<script src="ddbeforeandafter.js">
	
	/***********************************************
	* Before and After Image script (c) Dynamic Drive DHTML code library (www.dynamicdrive.com)
	* This notice MUST stay intact for legal use
	* Visit Dynamic Drive at http://www.dynamicdrive.com/ for this script and 100s more
	***********************************************/
	
	</script>
	
	<script>
	
	jQuery(function(){ // after DOM has loaded
		bafinstance = new ddbeforeandafter({
			wrapperid: 'baf'
		})
	})
	
	</script>


*Step 3:* Then, add the below sample markup to your page:

	<div id="baf" class="beforeandafter" style="width:550px; height:413px; ">
	
	<div class="before">
	<img src="taipeibefore.jpg" />
	<span class="caption">BEFORE</span>
	</div>
	
	<div class="after">
	<img src="taipeiafter.jpg" />
	<span class="caption">AFTER</span>
	</div>
	
	</div>
	
	<div style="width:550px; margin-top:1em">
	
	<div style="overflow:hidden; margin-bottom:1em">
	<a href="#" onClick="bafinstance.unveil('100%'); return false" style="float:right">Show "after" image fully</a> <a href="#" onClick="bafinstance.unveil('0%'); return false">Show "before" image fully</a>
	</div>
	
	<div style="overflow:hidden; margin-bottom:1em">
	<a href="#" onClick="bafinstance.unveil('70%'); return false" style="float:right">Show "after" image 
	70%</a> <a href="#" onClick="bafinstance.unveil('20%'); return false">Show "after" image 
	20%</a>
	</div>
	
	</div>

## Before and After image script set up ##

See script project page for additional details on setup and documentation: <http://www.dynamicdrive.com/dynamicindex4/beforeandafter.htm>
