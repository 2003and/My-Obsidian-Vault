Dithering is a technique used in pixel art used to imitate more colors than there actually is in the palette provided. To achieve such effect, two or more colors are interchanging on a given chunk of space. 
>[!note]
>You can think of dithering as something akin to hachure in traditional artworks, because both use two interchanging colors to simulate smooth transition between the two!

Most popular way of dithering is using a checkerboard pattern, although [[Stylized dithering]] could also be used. You can change the amount of filled/empty pixels to change the proportions of the colors blended together.

>[!warning]
>Too much dithering might overload the sprite if the canvas is too small! (But if the canvas is big you can go nuts with it)

One case the dithering is very useful for is, as mentioned earlier, simulate a bigger palette with a limited color palette, which is also useful to create gradients. [^1]
Another thing dithering is used for is to add texture to an object. And, while the traditional checkerboard pattern is the easiest and most reliable way to dither, you can use [[Stylized dithering|other patterns or even entire shapes instead]]! This will still yield the same fake blending effect, but will give a different feel to the object's texture

The basic dithering pattern is also usually pretty simple to [[Dithering filters in gamedev|simulate in games]]! (sometimes even mid-runtime, if you're technically savvy enough)

An interesting way of dithering I didn't hear much about is [[Intertwined dithering|intertwined dithering]]. [^2] In fact, I have only read about it only once in a book called [[Pixel_Logic_-_A_Guide_to_Pixel_Art_by_Michael_Azzi_z-lib_org.pdf|"Pixel Logic"]], which has shown three occurrences of such a technique. 

[^1]:![[basic_dither_example.png|500]]
([bayer matrix](https://ru.wikipedia.org/wiki/%D0%A4%D0%B8%D0%BB%D1%8C%D1%82%D1%80_%D0%91%D0%B0%D0%B9%D0%B5%D1%80%D0%B0) 8x8 was used)
>[!note]
Notice that to change the proportions of mixed colors, the amount of dark/light pixels in the pattern increases and decreases. This is a common way of creating gradients in pixel art.

[^2]:don't be scared if you don't understand - me neither
	```slide-note
file:Pixel_Logic_-_A_Guide_to_Pixel_Art_by_Michael_Azzi_z-lib_org.pdf
page:123
scale:1
dpi:2
rect: W(0.22), H(0.435), W(0.555), H(0.16)```