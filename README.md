# coding3

<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(28).png" width="600px" height="300px" alt="lab00-01"/>
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(25).png" width="1000px" height="300px" alt="lab00-01"/>

## Inspiration
My original goal was to use GAN to generate something new, something that didn't quite fit into the usual form of existence. I found a tutorial on generating new Pokemon on Kaggle. This is very similar to my idea of using an existing image to create a similar image.

## I changed things
Original code using the pokemon data sets, I tried for scenery, dogs and cats, animal data sets, but I finally decided to switch to portrait data sets, because the generated results become ridiculous and funny, like a beautiful works of art, look at each of the generated image, and as if can see subtle face. Green, red, green color mapping is the dream: trance real and absurd.

I also changed the number of EPOCHS and tried the influence of different training times on the results: I found that the larger the epoch, the higher the resolution of the generated images and the clearer the images. The number of images per row per column was also tried. I also tried to adjust the batch and buffer. I adjusted the number of generate-res and increased the value, so the computer would have more calculation work. I also tweaked the optimizer's type and found that RMSprop, while slower than Adam, was a bit sharper.

<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(3).png" width="300px" height="300px" alt="lab00-01"/>
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(5).png" width="300px" height="300px" alt="lab00-01"/>
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(4).png" width="300px" height="300px" alt="lab00-01"/>
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(6).png" width="900px" height="900px" alt="lab00-01"/>

## The problem
I found something interesting in training-data= Np.0 (Training_data,(-1,GENERATE_SQUARE,GENERATE_SQUARE,IMAGE_CHANNELS) If -1 is adjusted to a positive number within 10, the color of the result will be warm; if -1 is adjusted to a negative number, the color of the result will be cold.
I also tried to replace some code with other code, but for some reason no results were generated and no errors were reported. I also tried to generate images every 5 trains, but that didn't work either
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(20).png" width="600px" height="600px" alt="lab00-01"/>
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(19).png" width="600px" height="600px" alt="lab00-01"/>

## feeling
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(26).png" width="600px" height="600px" alt="lab00-01"/>
<img src="https://github.com/RunqiZhao21031188/1/blob/main/%E4%B8%8B%E8%BD%BD%20(18).png" width="600px" height="600px" alt="lab00-01"/>
In this work, I tried to adjust the epoch to a different number. Finally, due to the limitations of web pages and equipment, I failed to debug the epoch to a suitable parameter. The number of epoch times did not reach a certain level, resulting in imperfect effect, but the resulting effect seemed to develop in the direction of art, with an abstract and random beauty.
