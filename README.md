# Documentation

Welcome front-end devs to the What If Media Group Documentation for our ever-so-beautiful websites! First things first, this doc is meant to provide a guide to keep all of our sites <i>consistent, managable </i>, and <i>flexible</i>. This will outline where all links should be placed, script locations, necessary scripts, Pushnami/Google Tag Manager/ArcaMax requirements, layout and container formatting, frameworks, versioning, QA, and much more we use to keep these sites running smoothly. So, without further ado...  

Our sites are set up so that there is a <b>Container</b> which corresponds to a <b>Layout</b>.

### Layout 
Layouts are home to the *skeletons* of the websites. They contain all of the CSS files, JavaScript files, and any necessary Advertisement requirements (Google Tag Manager, Pushnami). They **DO NOT** contain any specific stylistic component, rather, they include the general/base CSS required to format the *container* properly, but that is all. Aesthetics are handled directly in the *container*. 

Layouts contain four (4) main components.
1. Landing pages
	* Unique Landing page
	* Return Landing page
2. Midpath
3. TCPA
4. Exit Page

Each of these pages will contain their own necessary CSS and JavaScript files. These can be found below:


# HTML, CSS, and Javascript for Layouts

Since our sites are so complex, we have plenty of stylesheets and scripts that are required to keep them running. Here are the specific ones that are <b>necessary</b> for all sites as of September 24th, 2018. 

## Unique Landing Page
### Scripts
*jQuery*
<br/>
Most of our old sites are in fact using older versions of jQuery. However, moving forward we are going to be using the latest version of jQuery availible. 

	<script src="https://code.jquery.com/jquery-3.3.1.min.js" integrity="sha256FgpCb/KJQlLNfOu91ta32o/NMZxltwRo8QtmkMRdAu8="crossorigin="anonymous"></script>

*Framework - Bootstrap*
<br/>
ALL OF OUR SITES WILL BE UTILIZING THE BOOTSTRAP FRAMEWORK FROM NOW ON! Please always use Bootstrap syntax, this is huge for consistency and often results in issues that could have easily been avoided if Bootstrap had been used. We will be using the most current version of Bootstrap, which right now is 4.0 (as of September 24th, 2018).

	
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js" integrity="sha384-JZR6Spejh4U02d8jOt6vLEHfe/JQGiRRSQQxSfFWpi1MquVdAyjUar5+76PVCmYl" crossorigin="anonymous"></script>
	<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>


*RegPath*

	  <script type="text/javascript" src="[{offer_cdn_url}]/js/extend.js"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/moment.js"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/jquery.validity.min.js"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/RegPath.js?rev=20180420"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/jquery.cookie.min.js"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/jquery.validity.custom-output.js?rev=20180410"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/RegPath.Functions.js?rev=20180420"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/RegPath.PrepForm.js?rev=20180420"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/RegPath.PersonalInfo.js?rev=201804225"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/jquery.mask.min.js"></script>
      <script type="text/javascript" src="[{offer_cdn_url}]/js/RegPath.Pixel.js?rev=201704101403"></script> 

*Form Validation*
<br/>
We are using a validation JavaScript plugin, so be sure to include this in order ensure proper form validation. 

	<script src="[{offer_cdn_url}]/js/omgsweeps/validator.js"></script>  

*Recaptcha* 
<br/>
	
	<script src="https://www.google.com/recaptcha/api.js" async defer></script>

*Pushnami* 
<br/>
This is dependent on sales whether they need Pushnami or not. Often times, you will be making two versions of the site, one with Push and one without. 

		<script type="text/javascript">
		(function(document, window){
		    var script = document.createElement("script");
		    script.type = "text/javascript";
		    script.src = "https://api.pushnami.com/scripts/v1/pushnami-adv/5ad8f62e29cfb115a3295cc5";
		    script.onload = function() {
			Pushnami
			    .update({
				"pstag": "R-[{sequence_id}]",
				"aff_id": "[{aff_id}]",
				"email": "[{email}]"
			    })
			    .prompt()
		    };
		    document.getElementsByTagName("head")[0].appendChild(script);
		})(document, window);
		</script>




          
