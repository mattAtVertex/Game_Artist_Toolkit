# 3. Setting up a Night Time Scene

<h2>Overview</h2>
<p>In this objective, we're going to identify some of the key differences between&nbsp; a day time lighting set up and a night time lighting set up.</p>
<hr>
<p><iframe src="https://www.youtube.com/embed/XmkR2_tBO9g?rel=0" width="800" height="450" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe></p>
<hr>
<h2>Fog</h2>
<p><a href="https://www.dropbox.com/s/fn7rsoxvf0nyetu/Vertex%20Handout_%20Environment%20Fog%20in%20Unreal.pdf?dl=0">Download this PDF Handout</a> for the full info on Fog in Unreal to help in understanding how best to use it in your scene.</p>
<p>The excerpt details below cover some of the major points:</p>
<h3>Exponential Height Fog</h3>
<p>The Exponential Height Fog is your premiere source of fog in the scene. Volumetric fog is going to be the bread and butter of any realistic exterior scene.</p>
<h4>Basic Settings</h4>
<ul>
<li>
<strong>Fog Density</strong><span> - The global density factor. Remember the general number you set here, as we’ll often temporarily crank it up to 1.0 to judge effects then take it back down.</span>
</li>
<li>
<strong>Height Falloff</strong><span> - This controls how dense the fog is as height increases, but note that the </span><strong>value relation appears reversed</strong><span>. Lower this value to make the fog thicker up high and raise it to thin out the fog up top and bring the thickness cutoff lower.</span>
</li>
<li>
<strong>Height Offset</strong><span> - This is used to offset the origin point. This can be useful if your map is at a higher altitude and you need to raise the base of the fog to match.</span>
</li>
<li>
<strong style="font-family: inherit; font-size: 1rem;">Second Fog Data</strong><span> - This adds an extra layer of fog thickness with similar parameters as above.</span>
</li>
</ul>
<p>&nbsp;</p>
<h4>Primary Volumetric Fog Settings</h4>
<ul>
<li>
<strong>Scattering Distribution</strong><span> - This controls how much incoming light scatters in various directions. 0 scatters equally in all directions where 0.9 scatters predominantly in the light direction. You’ll typically get the most realistic effects on the lower end.</span>
</li>
<li>
<strong>View Distance</strong><span> - Arguably one of the most powerful parameters, this affects how far you can see the fog. This controls the illusion of the thickness of the fog.</span>
</li>
<li><span><strong>Albedo</strong> - The reflected color of the fog particles</span></li>
<li><span><strong>Emissive</strong> - the emissive light that the fog gives off</span></li>
</ul>
<p>&nbsp;</p>