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

Each of these pages will contain their own necessary CSS and JavaScript files. These can be found (#-here)


# HTML, CSS, and Javascript for Layouts

Since our sites are so complex, we have plenty of stylesheets and scripts that are required to keep them running. Here are the specific ones that are <b>necessary</b> for all sites as of September 24th, 2018. 

<b>Scripts</b>
<br/>
<i>RegPath</i>

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
          
