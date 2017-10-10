<p>The weather feed used within this template is based on the <a href="http://solutions.arcgis.com/defense/help/maow/" target="_blank">Military Aspects of Weather version 2 (MAoWv2)</a> template and the user should make sure they are familiar with this before continuing.</p>
<p>To set up the template, complete the following steps:</p>
<ol class="steps">
  <li>Open ArcCatalog.</li>    
  <li>Within the AirC2 location navigate to AirC2Weather - Geodatabase - OperationalWeather.gdb.</li>
  <li>Publish the OperationalData and OperationalWind Datasets as Image services to your AirC2 folder created during the <a href = "./Publish-2D-Services.md" target="_blank">Publish 2D Services</a> section.</li>
    <ol class="steps">
      <li> While publishing the image service in the service editor click the function tab and then manage.</li>
      <li>Navigate to the location of the Raster Functions folder on disk and add all the raster functions apart from Wind Magnitude and Direction.rft to the OperationalData service. Wind Magnitude and Direction.rft should be added to the OperationalWind service and should be the only one added.</li>			
    </ol>
  </ol>
<h3 class="icon-notebook">Note</h3>
<p>The Location of the AirC2Weather folder will have to be registered as a datastore with your server click <a href="http://server.arcgis.com/en/server/latest/publish-services/windows/overview-register-data-with-arcgis-server.htm" target="_blank">here</a> to learn more.  If this is not possible then the datasets can be copied to an enterprise Geodatabase but it has to be made sure that the AirC2Weather folder is a share that can be accessed as the mosaic dataset still needs connection to the original NetCDF data.</p>
<p>The above steps have covered how to use the sample data that is provided, however it is likely that you will want to use your own weather data for the area that you are interested in.  As previously mentioned the weather feed within this template is based on the <a href="http://solutions.arcgis.com/defense/help/maow/" target="_blank">MAoWv2</a> template and it is to here that you should refer if you want to change the data and area. The subjects of relevance are <a href="http://solutions.arcgis.com/defense/help/maow/get-started/setup-location/" target="_blank">Setting up the Template in a Different Location</a> and the <a href="http://solutions.arcgis.com/defense/help/maow/workflows/setup-custom/" target="_blank">Setting up the Template with your data</a> sections. For the editing of and the addition of the Operational Impacts the section on <a href="http://solutions.arcgis.com/defense/help/maow/workflows/op-impact/" target="_blank">Operational Impact Generation</a> section should be looked at.</p>