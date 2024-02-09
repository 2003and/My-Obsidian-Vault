# [Extra source](https://youtu.be/YfCNJ9aEh6Y)

This note will teach you some hints on what exact screen and sprite size you should use

Two factors affect our decision:
- FoV we want our players or admirers to have (for example, a strategy game would have a large FoV, whereas a Zelda-like RPG would have a smaller FoV)
- Pixel scale we want to show

Here are some example screen resolutions[^1] (author of the video often uses them): 
- 480x270
- 360x203
- 270x152
- 240x135
- 216x122
- 192x108

>[!warning]
>If you want to have a small FoV but don't want large pixels - draw sprites in larger resolutions! (like, instead of 16x16 resolution for a player or a tileset use something like 64x64)
>But don't overdo on that one! If the scale will be too large you will most likely burn out before finishing the piece

>[!note]
>In case you want to look what screen size the sprites will look good on, follow these steps
>- make a large canvas in any image editing software
>- create a few rectangles that are the size of the example resolutions (or your personal preferred resolution, of course)
>- take your sprites, preferably built into a prototype beforehand
>- try them on by dragging them onto different rectangles and see which rectangle fits it the most

[^1]: ![[Suggested resolutions.png]]
This is a more in-depth picture on different screen resolutions I found... somewhere and sometime, but I can't recall the source. Sorry about that