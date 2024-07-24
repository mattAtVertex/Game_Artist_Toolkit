# 5. Getting the Planks to the Engine

<h2>Overview</h2>
<p>In this module we're going to take our plank kit into Unreal for use. After getting our mesh, textures, and materials set up, we'll look at how we can turn 5 planks into 60 to conceal repetition. In the second part, we'll look at setting up an edge blend material to help the planks better blend into the ground.</p>
<hr>
<h3>Part 1: Using the Plank Kit in Game</h3>
<p><iframe src="https://www.youtube.com/embed/sgBmRyYqFRw?rel=0" width="800" height="450" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe></p>
<p>&nbsp;</p>
<h3>Part 2: Dither Edge Blending with the Terrain</h3>
<p><iframe src="https://www.youtube.com/embed/wppawESm1uM?rel=0" width="800" height="450" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"></iframe></p>
<p><iframe src="https://www.youtube.com/embed/v2wRWAfvnk0?rel=0" width="800" height="450" allowfullscreen="allowfullscreen" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" data-mce-fragment="1"></iframe></p>
<hr>
<h2>Resources</h2>
<ul>
<li><a href="https://www.dropbox.com/s/c00nzps19d2fkqn/PlankKit_ProjectFiles.zip?dl=0">Plank Kit Game Ready Files</a></li>
</ul>
<hr>
<h2>Creating and Using the Dither Edge Blend</h2>
<p>Using the Dither Temporal AA functionality in Unreal can be a simple and easy way to make your objects blend in with things like terrain a lot easier. The steps are easy:</p>
<ol>
<li>Create a Material Function</li>
<li>Summon the DitherTemporalAA node and multiply it my a scalar parameter<br><img src="https://vertexschool.instructure.com/courses/151/files/8763/preview?verifier=nfwWf0DBpHpApdrV7zw0DHkyd5bmfJRku9C0SemD" alt="MF_Dither_Make.jpg" width="700" height="639" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8763" data-api-returntype="File"><br><br>
</li>
<li>Feed the Material Function into the Pixel Depth Offset input of your Material Attributes<br><img src="https://vertexschool.instructure.com/courses/151/files/8762/preview?verifier=3LH5vpqTBqBwvNfu0brAS2uJz429dl5UqfN6RgyY" alt="MF_Dither_Use.jpg" width="700" height="617" data-api-endpoint="https://vertexschool.instructure.com/api/v1/courses/151/files/8762" data-api-returntype="File"><br><br>
</li>
<li>The DitherAmount parameter will now show up in your material instance to edit.
<ol>
<li>0 = Off, no edge blending</li>
<li>1 = Standard, like feeding the DitherTemporalAA node directly in</li>
<li>5 = Extreme value, try not to go over this value or you might content with some artifacts</li>
<li>1.5 - The ideal value in most situation</li>
</ol>
</li>
</ol>
<p>&nbsp;</p>