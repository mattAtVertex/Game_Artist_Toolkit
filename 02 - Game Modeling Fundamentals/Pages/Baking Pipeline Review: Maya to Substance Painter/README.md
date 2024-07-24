# Baking Pipeline Review: Maya to Substance Painter

<h2>Part 1: Setting Up Color IDs in Maya</h2>
<p><iframe src="https://www.youtube.com/embed/WPAn3XWVpLA?rel=0" width="960" height="540" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe></p>
<hr>
<h2>Part 2: Export Set Up for Baking</h2>
<p><iframe src="https://www.youtube.com/embed/KcevOHZG2pc?rel=0" width="960" height="540" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe></p>
<hr>
<h2>Part 3: Baking in Substance Painter</h2>
<p><iframe src="https://www.youtube.com/embed/nBbiAcbT_YQ?rel=0" width="960" height="540" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe></p>
<h3>The Interface</h3>
<p>When you open Substance Painter you will be greeted with a blank canvas. Let’s define some of the areas.</p>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8694/preview?verifier=5OG98HNpfahqErvZ6CluFQkrmqHsY7jOv77ltV2n" alt="interface.jpg" width="640" height="360" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8694" data-api-returntype="File">&nbsp;&nbsp;</p>
<p>&nbsp;</p>
<h3>Interface Areas</h3>
<ul>
<li>
<strong>Viewports</strong><span> are where you will see the model upon import. You can manipulate the viewports with the familiar “Maya” style navigation. ALT+LMB rotate : ALT+RMB zoom (or scroll wheel) : ALT+MMB pan</span>
</li>
<li>
<strong>Viewport Tools</strong><span> manipulate the viewports as well as the imported model.</span>
</li>
<li>
<span>The </span><strong>Brush and Selection Tools</strong><span> operate within the viewports on your model.</span>
</li>
<li>
<span>The </span><strong>Active Tab Panel </strong><span>displays information related to the tabs across the top of the window.&nbsp;</span>
</li>
<li>
<span>The </span><strong>Properties Panel </strong><span>displays the properties and options available based on what is selected in the Active Tab. </span>
</li>
<li>
<strong style="font-family: inherit; font-size: 1rem;">The Library</strong><span> is a collection of tools, materials, and utilities that alter your model or viewport.</span>
</li>
</ul>
<hr>
<h3>Creating Your Project</h3>
<p>To start, let’s create a New File.</p>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8693/preview?verifier=i6rvWrsaiHbx8Oq0zySm9GhnfrtyRIYeFN3kwYjP" alt="fileNew.png" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8693" data-api-returntype="File">&nbsp;&nbsp;</p>
<ol>
<li><span>In the New Project window: Select the Unreal Engine 4 (Allegorithmic) template from the drop-down box as we will be importing these into Unreal later.</span></li>
<li><span>Click the “Select…” box. Here you will navigate to your low poly models .FBX file. This will be the imported mesh.</span></li>
<li><span>Leave the Document Resolution at the default setting. This setting can be changed at any time, as Painter is non-destructive and only encodes the resolution on export.</span></li>
<li><span>Normal Map: Set to DirectX </span></li>
<li><span>Leave all other settings at default.&nbsp; AutoUVUnwrap is checked.&nbsp; Compute tangent… is checked.</span></li>
<li><span>Click OK. Your mesh will now import and you will have something resembling the first image, where your model is in the viewport. Now we are ready to start baking the maps!</span></li>
</ol>
<p>&nbsp;</p>
<h3>Baking Mesh Maps Using Match By Name (The Preferred Approach)</h3>
<p><span>Initializing the baker window. Edit &gt; Bake Mesh Maps.&nbsp;</span></p>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8692/preview?verifier=ydDlrMykz44Yt8d2Vwuk7wG6S5WxRWYhWAnYmN8r" alt="BakerWindow.jpg" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8692" data-api-returntype="File">&nbsp;&nbsp;</p>
<ol>
<li><span>Set the Output Size to 2048.</span></li>
<li><span>Select your High Definition Mesh and click the little paper icon.&nbsp; This will allow you to select your high-resolution mesh.</span></li>
<li><span>Set Max Frontal and Max Rear Distance to 0.07</span></li>
<li><span>Set Anialiasing to Subsampling 4x4.</span></li>
<li><span>Set Match to By Mesh Name.</span></li>
<li><span>Check the ID box (The ID parameters will show up)</span></li>
<li><span>Set Color Source to Mesh ID/Polygroup.</span></li>
<li><span>Set Color Generator to Random.</span></li>
<li><span>Click Bake 1001 Mesh Maps.</span></li>
</ol>
<p>When the Baker is done it's time to check the maps for issues.</p>
<p>&nbsp;</p>
<h3><span>Common Problems</span></h3>
<ul>
<li><span>Missing parts of the map: check your Max frontal/Rear Distance settings.</span></li>
<li><span>Maps are not showing: check to see if the missing map is ticked in the baker window.</span></li>
<li>
<span>Maps still not showing:</span>
<ul>
<li dir="ltr"><span>Confirm your mesh names are set: _high and _low.</span></li>
<li><span>And Match: By Mesh Name.</span></li>
</ul>
</li>
<li><span>ID is not showing: check to see if Color Source is set to Mesh ID/Polygroup.</span></li>
<li><span>Stretching: check your UVs.</span></li>
<li>
<span>Artifacting:</span>
<ul>
<li><span>check your Max frontal/Rear Distance settings.</span></li>
<li><span>check your hard/soft edges in Maya.</span></li>
</ul>
</li>
</ul>
<p><span>&nbsp;</span></p>
<p><span>This Quick Start Guide is the general workflow for successful baking in Substance Painter.</span></p>
<p>&nbsp;</p>