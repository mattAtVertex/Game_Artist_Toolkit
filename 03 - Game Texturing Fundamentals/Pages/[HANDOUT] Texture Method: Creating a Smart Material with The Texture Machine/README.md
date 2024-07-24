# [HANDOUT] Texture Method: Creating a Smart Material with The Texture Machine

<h1><span>Creating a Smart Material with Substance Painter</span></h1>
<p><span><img src="https://vertexschool.instructure.com/courses/151/files/8721/preview?verifier=jKdn9TuMPtNNhHK4tGYC4wLjRBLDqLGzCVKqCgpW" alt="image10.png" width="1999" height="1092" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8721" data-api-returntype="File"></span></p>
<h2><span>Overview</span></h2>
<p><span>In this handout, we’re going to dive headfirst into Substance Painter and create our first smart material. Substance Painter has often been described as a 3D version of Photoshop. Let’s have a look at how we can take advantage of familiar workflows to create a smart material.</span></p>
<p>&nbsp;</p>
<h2><span>Prerequisites</span></h2>
<p>&nbsp;</p>
<ul>
<li><span>Substance Painter installed and ready to go</span></li>
<li><a href="https://drive.google.com/file/d/1bmNuyTPk-swYkIM42BZW55tqBurpMttT/view?usp=sharing"><span>Download and unzip Mesh MAT to get the FBX</span><span><br></span></a></li>
</ul>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8700/preview?verifier=mxmvUlOXnRnDxW2V2IvP27OBT8bDgnJ2Fl27y92S" alt="image4.png" width="789" height="69" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8700" data-api-returntype="File"><br><br></p>
<p><span>Once everything is ready, continue to the next page to get started.</span></p>
<p>&nbsp;</p>
<h1><span>Creating the Smart Material</span></h1>
<h2><span>New Project Setup</span></h2>
<p><span>Before we can create our Smart Material, we need to get set up with a new project. In order to create a material, you need a mesh to view it on. Since we’re creating a Smart Material that is going to be tileable and reusable, we can go ahead and build it using a common starting point: MAT. Make sure you have downloaded the Zip from the prerequisites section and extracted the FBX.</span></p>
<p>&nbsp;</p>
<ol>
<li>
<span>Select</span><strong> File &gt; New</strong><span> to create a new project.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8725/preview?verifier=55EszbbGs1rxD8NO2H6BvMsPCx5DhsH1b7f0c7wz" alt="image2.png" width="626" height="129" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8725" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>This will open the </span><strong>New Project</strong><span> dialog. Just a few quick things here and we’ll be ready to go.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8715/preview?verifier=cTD7sTnoHxBgl80Qat5ar5DkGWqTaseK0uDH8wAI" alt="image19.png" width="1178" height="646" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8715" data-api-returntype="File"><br><br></span>
</li>
<ol>
<li>
<strong>Select button</strong><span> and navigate to your </span><strong>Mesh_Mat.fbx</strong><span>. This is going to be the mesh you are working on. In a typical workflow, this would be your Low Poly.</span>
</li>
<li>
<span>Make sure your </span><strong>Document Resolution</strong><span> is set to a manageable size like 2048. Even when planning to export as 4k, it’s good to keep your working document size reasonable because you will be working with several layers. This can eat up your RAM fast.</span>
</li>
<li>
<span>Hit the </span><strong>OK button</strong><span> to finish the New Project setup.</span>
</li>
</ol>
<li>
<span>Substance Painter will now load up your main workspace with the MAT mesh and you should be ready to go!</span><span><br></span>
</li>
<li>
<span>Let’s have a quick look at the interface and make note of our primary areas.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8707/preview?verifier=8rMSfLK9kQ4TW3U6sguFbLVImAgf758fqQvQNEVl" alt="image6.png" width="1999" height="1125" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8707" data-api-returntype="File"></span><span><br></span><strong>Viewport</strong><span> - This is your main workspace. This is where you will see your model.</span><span><br></span><strong>Layer Stack</strong><span> - This is where you will layer textures to create your machine.</span><span><br></span><strong>Details</strong><span> - This is where you will adjust parameters for materials, brushes, masks, and generators.</span><span><br></span><strong>Shelf</strong><span> - This is your library collection of things like materials, brushes, and tools.</span><span><br><br></span>
</li>
<li>
<span>Before we can start the texturing process, we need some basic helper maps to work with. We don’t have a high poly, but we can use the low poly as a high poly to bake these maps. Switch to the </span><strong>Texture Set Settings</strong><span> tab and find the </span><strong>Bake Mesh Maps</strong><span> button. This will open the Baking dialog.</span>
</li>
<li><span>In here, make sure the document resolution is set to at least the size of your working resolution. In this case, we can use 2048.</span></li>
<li>
<strong>Uncheck the ID option</strong><span>. We don’t have a high poly with material IDs, so we have nothing to bake. If we leave it checked, we’ll get a warning. The warning won’t hurt anything, but it’s best to get yourself in the mindset of only baking the maps you need.</span>
</li>
<li>
<span>Check the </span><strong>Use Low Poly as High Poly Mesh</strong><span> option. This is where the magic happens. Since we don’t have a high poly version, we can bake the low poly onto itself. This will still give us all of the helper maps we need like Curvature, Position, and AO.</span>
</li>
<li>
<span>When you’re done with these settings, hit the </span><strong>Bake all Texture Sets</strong><span> button to start baking.</span>
</li>
</ol>
<p><span><img src="https://vertexschool.instructure.com/courses/151/files/8703/preview?verifier=1J6Fb1MiDBqZpasKs34SHVHFFNeWjVJId3MS2KZw" alt="image24.png" width="1765" height="999" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8703" data-api-returntype="File"><br><br></span></p>
<p><span>Now you should be all set up. Next, we’re going to start creating a smart material.</span></p>
<p><br><br><br></p>
<h2><span>Understanding Layers</span></h2>
<p><span>Before we move forward, we need to understand the two types of layers.</span></p>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8734/preview?verifier=lAzvFw013HOPqCeDNQ8PNhe4EtWDNjLPkMJxSP1t" alt="image21.png" width="696" height="228" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8734" data-api-returntype="File"><br><br></p>
<p><strong><img src="https://vertexschool.instructure.com/courses/151/files/8717/preview?verifier=TYkI4shOqMUhCYI3rW4DjCbk5bbxyi1YZdSP4L3Y" alt="image11.png" width="37" height="29" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8717" data-api-returntype="File">&nbsp;Paint Layers </strong><span>&nbsp;- Layers that you can paint directly in. No texture map assignments, just raw paint with a brush.</span></p>
<p><strong><img src="https://vertexschool.instructure.com/courses/151/files/8718/preview?verifier=er8B448N8dKaKBCFHJbYGvY6kpRpSqNOz7s3mfsM" alt="image36.png" width="37" height="29" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8718" data-api-returntype="File">&nbsp;Fill Layers</strong><span> - Material Layers that contain slots for each texture map. You cannot paint on these layers.</span></p>
<p><strong>Fill Layers</strong><span> are going to be one of our biggest assets in building textures. These layers allow us to assign a value -- or even a 2D texture map like a grunge or noise pattern -- to the</span><strong> individual texture channels</strong><span> of the material. You can even </span><strong>toggle what channels you want to use</strong><span> with that layer.&nbsp;</span></p>
<p>&nbsp;</p>
<p><span>We also have control over the </span><strong>UV tiling, position, and rotation</strong><span> options.</span></p>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8723/preview?verifier=yoNz17VCSypjnieZtnYWZaf64HJZcSxI2EHai7pZ" alt="image27.png" width="1067" height="911" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8723" data-api-returntype="File"><br><br></p>
<p><span>The </span><strong>Material Mode</strong><span> slot also allows us to drop a premade material directly into this layer. The premade material will then take over control of the individual channel slots. These premade materials are usually created separately in </span><strong>Substance Designer</strong><span>.</span></p>
<p>&nbsp;</p>
<p><span>Now that we’re familiarized with the fill layer, we can start using it to build our material.</span></p>
<h2><span>Creating the Base Material</span></h2>
<p>&nbsp;</p>
<ol>
<li>
<span>We’re going to start by creating a Fill Layer and naming it Base Material. This will be the initial definition of our smart material.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8708/preview?verifier=zFCtPuuDRqPZMteIrjsIsWzCeVF2RkJWxtjwjA1P" alt="image18.png" width="411" height="176" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8708" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>In the </span><strong>Shelf</strong><span>, type “</span><i><span>concrete</span></i><span>” into the search bar to find all of the installed concrete materials. With the </span><strong>Base Material</strong><span> layer selected in the </span><strong>Layer Stack</strong><span>, double click the </span><strong>Concrete Simple</strong><span> material. This will assign it to the layer.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8704/preview?verifier=7L4ArcMPvXdtGnrHTb4VY23grLXrRm5d3QJHHTLh" alt="image1.png" width="1684" height="711" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8704" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>Next, we want to make sure that this material stack is organized properly. With the Base Material layer still selected, Hit </span><strong>Ctrl + G</strong><span> to put it into a </span><strong>Folder Group</strong><span>. We can name this folder something like “Smart Concrete”</span>
</li>
<li>
<span>Next, create a new </span><strong>Fill Laye</strong><span>r above base material inside of the folder, and name it “Value Variation”.<br><img src="https://vertexschool.instructure.com/courses/151/files/8720/preview?verifier=zhmK5RKou04AWJwKxZceMw9IJJsBTCaDBmQ5AtRj" alt="image29.png" width="391" height="191" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8720" data-api-returntype="File"><br></span><span><br></span>
</li>
<li>
<span>In the properties, </span><strong>Alt + Click</strong><span> the </span><strong>color</strong><span> option to deselect every other channel except color. You should only see the </span><strong>Base Color</strong><span> slot now. Click on this to bring up the texture menu. Now type “grunge” into the search box. You should see a bunch of grunge textures show up.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8731/preview?verifier=2YuN2n8QpsdwDgKQNMfqR6YBWRwZ1X6tfOtC83xx" alt="image20.png" width="378" height="346" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8731" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>Pick a grunge texture you like. </span><i><span>Grunge Concrete Old</span></i><span> is a good one for this purpose. When you select it, it will be assigned to the Base Color channel.&nbsp;</span>
</li>
<li>
<span>Back up in the </span><strong>Layer Stack</strong><span>, let’s change the </span><strong>blend mode to Overlay</strong><span> and set the </span><strong>Opacity to around 28%</strong><span>. We’re aiming for subtlety. This opacity value can vary greatly depending on the grunge texture that you use.&nbsp;</span>
</li>
<li>
<span>Even at a low opacity, the subtle variation will make a huge difference.You can toggle the layer display on and off to visually see the difference.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8710/preview?verifier=chk5hIF5qDdVFuaZO7MMKvDUzX4qs7gBMZI07yOl" alt="image25.png" width="1402" height="519" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8710" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>Next, we’re going to add another variation layer, except this time we’re going to focus on </span><strong>Roughness</strong><span>. Create another </span><strong>Fill Layer</strong><span> and name it “Roughness Variation”.</span>
</li>
<li>
<span>In this layer, </span><strong>Alt + Click</strong><span> the </span><strong>rough</strong><span> option to deselect all the other channels. Just like before, click on the Roughness slot and select a grunge texture. </span><i><span>Grunge Dirt Large</span></i><span> is a good one for this example.</span>
</li>
<li>
<span>Now, since we’re working with the </span><strong>Roughness Channel</strong><span> now, we need to make sure we are working in the correct channel in the Layer Stack. Find the </span><strong>channel selector dropdown</strong><span>&nbsp; at the top of the Layer Stack. It should say Base Color. Click this and select Roughness. We are now editing the roughness channel in the Layer Stack.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8729/preview?verifier=5gwguedgzoLzyHL1RImsXhK7rQH16s4ksmaBl6Hk" alt="image8.png" width="952" height="287" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8729" data-api-returntype="File"></span><span><br></span><span><br></span><span>Also note that you can change the currently viewed material on the mesh in the viewport to individual channels. This can help with tweaking values.</span>
</li>
<li>
<span>Let’s go ahead and change our </span><strong>blend mode to Multiply</strong><span> and </span><strong>Opacity to around 45%</strong><span>. You want a subtle effect, so this opacity can vary greatly depending on the grunge texture that you use.</span>
</li>
<li>
<span>Now in the viewport, hold down </span><strong>Shift + Right Click</strong><span> and move the mouse around to adjust the rotation of the light to check the results.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8712/preview?verifier=xk83iarqU2qXwU6toXhc1DctpuIz2648TqcDIrPu" alt="image12.png" width="1677" height="547" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8712" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>To finish up the base, we need to add some color variation as well. So let’s go back to working in the </span><strong>Base Color</strong><span> for the </span><strong>Layer Stack</strong><span>.</span>
</li>
<li>
<span>Create a new</span><strong> Fill Layer</strong><span>. Name it “Color Variation”. In the details panel, just like the value variation,</span><strong> Alt + Click</strong><span> the </span><strong>color </strong><span>option to toggle off all the other channels.&nbsp;</span>
</li>
<li>
<span>Next, Click on the </span><strong>Base Color</strong><span> slot to select a </span><strong>high contrast grunge</strong><span> texture. </span><i><span>Grunge Map 001</span></i><span> works great for this example.</span>
</li>
<li><span>We’re going to do something a little different with this layer. We’re going to add a gradient filter to control color variation based on the grunge texture that we chose.</span></li>
<li>
<span>Right click the Color Variation layer and select </span><strong>Add Filter</strong><span> towards the bottom.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8706/preview?verifier=c7g69nxg0WANkUoLwFnBxgjCfR6In6D4czKPDCUx" alt="image34.png" width="347" height="125" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8706" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>In the details panel, toggle off all the other channels besides color. Then click on the </span><strong>Filter slot</strong><span> and select </span><strong>Gradient</strong><span> from the list.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8705/preview?verifier=uwlbguvLcOH9b9T2m7D5Tw0fkbWqBv41MT6ivUeU" alt="image35.png" width="911" height="321" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8705" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>In the settings for the filter, you’ll see 3 color swatches of black, gray, and white. You can click on these to change the color. The colors will be applied to the corresponding grayscale value in the grunge map you chose as a gradient. You want to utilize strong colors in this step. We can tweak them in the next part.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8724/preview?verifier=debNI97240MrmsHOc0aegI2bE0CuVcTdAi6hJOUs" alt="image32.png" width="1588" height="760" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8724" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>With colors chosen, go back to the layer stack and change the </span><strong>blending mode to Overlay</strong><span>. Then drop the </span><strong>opacity down to around 24%</strong><span>. You’ll see we now have a subtle color variation to the material. With the blending and opacity set, you can tweak the colors as need be to get the result that you want.</span>
</li>
<li>
<span>Once again, we’re aiming for subtlety. You can toggle on and off the visibility of the color variation layer to see the difference the effect adds.</span><span><br></span><span><br></span><span>In the image below, take note of how the subtle color variation affects the both the base color and the specular highlighting.</span>
</li>
</ol>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8732/preview?verifier=1Q3LliTzMIDrhibZsYV2USn7Zlq3ZPLziSvhbpWg" alt="image5.png" width="1999" height="851" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8732" data-api-returntype="File"><br><br></p>
<h2><span>Adding Some Dirt</span></h2>
<p><span>Our material is already looking pretty good, but we can take it a little bit further by adding a dirt layer. In this section, we’re going to get an introduction to masks and generators.</span></p>
<p>&nbsp;</p>
<p><span>Before moving forward, let’s just verify that our layer stack is looking right. We should have a Base Material, Value Variation, Roughness Variation, and Color Variation with a gradient.</span><span><br><img src="https://vertexschool.instructure.com/courses/151/files/8722/preview?verifier=7GJONVsQhCxa22Qg8EpxzN8iWfjoFhj9yn43QElc" alt="image22.png" width="330" height="342" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8722" data-api-returntype="File"><br></span></p>
<p><span>Looks good? Alright, let’s get started.</span></p>
<p>&nbsp;</p>
<ol>
<li>
<span>Create a new </span><strong>Fill Layer</strong><span>. Name this layer “Dirt”.</span>
</li>
<li>
<strong>Alt + Click</strong><span> color to toggle all the other channels off, just like before. We’ll be working with just the color to start.</span>
</li>
<li>
<span>Now in the Base Color slot, pick a good dark grunge. Any of the grunge dirt textures will work for this. </span><i><span>Grunge Dirt Thin</span></i><span> is a favorite for this.</span>
</li>
<li>
<span>The grunge texture looks a little large for this purpose, so we want to scale the UV tiling just a bit. Find Scale in the parameters in the detail panel and set it to 2. Notice how the texture on the model changes.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8706/preview?verifier=c7g69nxg0WANkUoLwFnBxgjCfR6In6D4czKPDCUx" alt="image34.png" width="347" height="125" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8706" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>With our dirt layer setup, let’s apply it to the model in a reasonable format. We’re going to do this procedurally through the use of a generator. But first, we need to define a mask to work with. </span><strong>Right click</strong><span> the Dirt Layer in the Layer Stack and choose</span><strong> Add a Black Mask</strong><span>. You’ll notice the dirt texture goes away and there is a mask assigned.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8714/preview?verifier=RJnueuHkAcfb0qjjjNTov4JnhWfHd5SJstuIfpQP" alt="image30.png" width="348" height="79" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8714" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>We want to use a generator to procedurally reveal parts of this layer. Making sure the </span><strong>mask icon</strong><span> is still selected, right click and click </span><strong>Add Generator</strong><span>.</span>
</li>
<li>
<span>Make sure the generator option is selected in the Layer Stack. In the details panel, click the Generator slot and find the Dirt generator.<br><img src="https://vertexschool.instructure.com/courses/151/files/8730/preview?verifier=FcMpk2pIKNF9Rt2rS8O0cYPCqvWqoIk0y5FvghFZ" alt="image28.png" width="781" height="251" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8730" data-api-returntype="File"><br></span><span><br></span>
</li>
<li>
<span>Notice how the mask is altered and we see our dirt layer showing up in the crevices of the mesh. </span><span><br></span><span><br></span><span>Remember how we baked the low poly mesh onto itself earlier? Even without a high poly, the maps that the baking process creates (such as </span><strong>Curvature</strong><span>, </span><strong>Ambient Occlusion</strong><span>, and </span><strong>Position</strong><span>) are vital to making these generators work. Without them, the generators would be all but useless.</span>
</li>
<li>
<span>This is a pretty cool start, but let’s have a look at some of the settings for the dirt generator. Looking in the detail panel, we can find a few settings that are going to be our core tweaks:</span><span><br></span><span><br></span><strong>Dirt Level</strong><span> - this controls the global amount of dirt, brightening the mask.</span><span><br></span><strong>Dirt Contrast</strong><span> - this controls the global contrast of the dirt mask</span><span><br></span><strong>Grunge Amount</strong><span> - This controls the blend of the grunge, which is a default internal grunge texture </span><span><br></span><strong>Grunge Contrast</strong><span> - This controls the contrast of the internal grunge texture.</span><span><br></span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8711/preview?verifier=a22qJWB0uUZnffgVUfAzW94ELFjklgZcezxbJlcv" alt="image9.png" width="932" height="438" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8711" data-api-returntype="File"></span><span><br></span><span>Also note that you can scroll to the bottom to see where you can use a custom grunge texture to replace the internal default grunge if you want.</span>
</li>
<li>
<span>To finish off setting up the color layer, start taking the </span><strong>opacity </strong><span>of the layer down to get a good blend.</span>
</li>
<li>
<span>Next, click on the layer icon to get back to the fill layer settings.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8716/preview?verifier=FDBPxE7NT6nptUJ1m2Qdl5f0L1AZsScpfIw4sCSw" alt="image7.png" width="350" height="71" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8716" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>With our dirt mask set up and our color layer blended, let’s do something with the roughness.Click the </span><strong>rough </strong><span>option to toggle the roughness channel on for this layer.<br><img src="https://vertexschool.instructure.com/courses/151/files/8713/preview?verifier=yxEyOaaWOQgpwfLouR8Whm2uJSBN48nCt7UijigB" alt="image26.png" width="309" height="56" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8713" data-api-returntype="File"><br></span><span><br></span>
</li>
<li>
<span>Now, click on the newly revealed </span><strong>Roughness</strong><span> slot and pick a primarily white grunge texture. </span><i><span>Grunge Sand Dry</span></i><span> works great here. Tweak the </span><strong>Balance </strong><span>and </span><strong>Contrast </strong><span>until you get some nice white spots showing up in your roughness channel where the dirt mask shows.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8726/preview?verifier=x3CtS5HHPjkdGZtP6xzvPVFX9eSsWIzLJzazHpOt" alt="image37.png" width="331" height="208" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8726" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>Back in the Layer Stack, switch to the </span><strong>Roughness Channel</strong><span> and set the </span><strong>blend mode</strong><span> for the dirt layer’s roughness to </span><strong>Screen</strong><span>. Then take the opacity down just a bit to get a good blend, but we still want the dirt areas to be fairly bright in the roughness channel.<br><img src="https://vertexschool.instructure.com/courses/151/files/8733/preview?verifier=go4eP9lZ8Q9mBA5cFY6fpKUhJFCidoKGx7BWuxDZ" alt="image23.png" width="345" height="148" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8733" data-api-returntype="File"></span><span><br></span>
</li>
</ol>
<p>&nbsp;</p>
<p><span>Awesome! Now our material is a little bit more exciting. Check the </span><strong>Before and After</strong><span> below to see how much of a difference these </span><strong>subtle changes</strong><span> actually make when combined together. When building textures like this, remember that a little bit goes a long way and there is never just one magic bullet. It’s a lot of little details that all work together to create the final look.</span><span><br><br></span></p>
<p><span><img src="https://vertexschool.instructure.com/courses/151/files/8728/preview?verifier=xM9rFYUpbb3E8ybtaBTmrnoRHTA8SLGvLnQ6kdm6" alt="image16.png" width="1999" height="841" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8728" data-api-returntype="File"></span></p>
<p>&nbsp;</p>
<h2><span>Turning it all into a Smart Material</span></h2>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8709/preview?verifier=RuZNeOvE8qUdml1gnjBGGTzP5sX1seHUWF44wEr9" alt="image14.png" width="1546" height="1024" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8709" data-api-returntype="File"></p>
<p><span>It’s Ok, MAT. We just have one more step. We created the material, now let’s turn it into a </span><strong>Smart Material</strong><span>. The process is really easy. Any </span><strong>Folder Group</strong><span> in the layer stack can be turned into a Smart Material.</span></p>
<p>&nbsp;</p>
<ol>
<li>
<span>Right click the Smart Concrete folder in the layer stack and select </span><strong>Create Smart Material</strong><span>.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8691/preview?verifier=NRBHCkcsYAUEc5JZQwuKwnOMCBcd74oBDwTYMvhw" alt="image15.png" width="894" height="56" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8691" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>You should now see in the </span><strong>Smart Materials</strong><span> section of the </span><strong>Shelf</strong><span>, our Smart Concrete shows up.</span><span><br></span><span><img src="https://vertexschool.instructure.com/courses/151/files/8702/preview?verifier=8btadtWYzGWWk1HpqrRTgimvaN1hFWlaL2V9ZDMR" alt="image13.png" width="1259" height="264" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8702" data-api-returntype="File"><br><br></span>
</li>
<li>
<span>Now, back up near the Layer Stack, click the Texture Set List icon to reveal the texture set list. Here you can see all of the materials assigned to the mesh. In MAT’s case, we have Head, Body, and Base. Go ahead and select </span><strong>02_Body</strong><span>. Note that you can freely switch between texture sets.<br><img src="https://vertexschool.instructure.com/courses/151/files/8727/preview?verifier=1SjsXR1VRoItSaY71SuHjmfwgIsXoqggGO6eoMeB" alt="image17.png" width="451" height="228" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8727" data-api-returntype="File"><br></span><span><br></span>
</li>
<li>
<span>The first thing you will notice is that the layer stack is empty. That’s because we are working on a different material. We want to use our </span><strong>Smart Material</strong><span> on the body. So Grab the Smart Concrete material from the shelf and drop it onto the body in the viewport. Notice how it creates a folder just like we had before in the layer stack.<br><img src="https://vertexschool.instructure.com/courses/151/files/8701/preview?verifier=dOA5FMfFQeVLTJ11XyZQcEd2LyX2ZwEw1TqmuLYS" alt="image31.png" width="1254" height="527" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8701" data-api-returntype="File"><br></span><span><br></span>
</li>
<li>
<strong>Repeat </strong><span>the process for the </span><strong>03_Base</strong><span> material set too.</span>
</li>
</ol>
<p>&nbsp;</p>
<p><span>Congrats! You have created a smart material and applied it to multiple texture sets. There’s still a lot to do with gradients and environmental effects, but your smart material makes a solid starting point for new projects.</span></p>
<p><img src="https://vertexschool.instructure.com/courses/151/files/8719/preview?verifier=EdFXaxPcZ2Cysi5yDthrzpm4JWrrBi2ymSpacT2O" alt="image3.png" width="1680" height="994" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8719" data-api-returntype="File"></p>
<h1><span>On Your Own</span></h1>
<p><span>Now that you know how to work with the </span><strong>different variations</strong><span> to create a nice texture and turn it into a </span><strong>Smart Material</strong><span> to reuse, try creating one on your own. Create something with stone, wood, metal, or leather.&nbsp;</span></p>
<p>&nbsp;</p>
<p><span>Remember these </span><strong>core variations</strong><span> we learned about in this worksheet:</span></p>
<p>&nbsp;</p>
<ul>
<li><span>Value variation</span></li>
<li><span>Color Variation</span></li>
<li><span>Roughness Variation</span></li>
</ul>
<p>&nbsp;</p>
<p><span>These are a set of parts to the process of creating “</span><strong>The Texture Machine</strong><span>” and are going to be a key aspect of any texture job you do.</span></p>
<p>&nbsp;</p>
<h2><span>Exercise</span></h2>
<p>&nbsp;</p>
<ol>
<li><span>Create a Smart Material made of stone, wood, metal, leather, or any material that might be useful to your Capstone project.</span></li>
<li><span>Experiment with other generators (such as the Metal Edge Wear generator).</span></li>
<li><span>Think about the type of usage this material might generally have and consider how that might affect your variations or your dirt layers.</span></li>
<li><span>Try using your smart material on a new mesh in a new project.</span></li>
<li><span>Share your results.</span></li>
</ol>
<hr>
<h3>Resources</h3>
<ul>
<li style="list-style-type: none;">
<ul>
<li><a class="external" href="https://drive.google.com/file/d/1bmNuyTPk-swYkIM42BZW55tqBurpMttT/view?usp=sharing" target="_blank"> <span>Mesh MAT FBX</span></a></li>
</ul>
</li>
</ul>