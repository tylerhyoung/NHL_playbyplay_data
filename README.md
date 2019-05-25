# NHL_playbyplay_data
This is a side project I'm working on where I gather data from the NHL api to make interesting analysis and visualizations.

https://public.tableau.com/views/NHLShotComparison/ShotComparer?:embed=y&:display_count=yes&:origin=viz_share_link

<!-- JS file to enable the JavaScript API. You can point at the
  version on public.tableau.com, online.tableau.com, or your on-prem Server -->
<script src="https://public.tableau.com/javascripts/api/tableau-2.min.js"></script>
...
<!-- Empty div where the viz will be placed -->
<div id="tableauViz"></div>     

function initializeViz() {
  // JS object that points at empty div in the html
  var placeholderDiv = document.getElementById("tableauViz");
  // URL of the viz to be embedded
  var url = "https://public.tableau.com/profile/tyler.young#!/vizhome/NHLShotComparison/ShotComparer";
  // An object that contains options specifying how to embed the viz
  var options = {
    width: '600px',
    height: '600px',
    hideTabs: true,
    hideToolbar: true,
  };
  viz = new tableau.Viz(placeholderDiv, url, options);
}
