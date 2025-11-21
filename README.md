# Trackmania PBRTv4 Render

PBRTv4 code of trackmania cars driving down a highway \
I tried to make the cars look in motion by adding dust trails behind them that they've kicked up

## Final Renders
- the final renders are in the `final_render` folder
- these are two 4K images rendered with 2048 samples per pixel
- the second render is just a little lighter if you wanted to see the details better

![cars driving down a highway at night](./final_renders/4k_2048_dark.png)\
![cars driving down a highway at night](./final_renders/4k_2048_light.png)

## What is PBRT?
Path Based Ray Tracing is a way of rendering images in which each rays from the camera are simulated in the world, interacting with objects by bouncing off them or getting absorbed (or both!). Each rendered pixel is the average of $N$ rays shout out at slighlty different angles, and then all averaged together. The more rays you shoot our per pixel, the less noisy the image becomes, as more data is used to create each pixel. Due to this, rendering a high quality 4k image can take a *lot* of computer power. Two images in this repo are rendered at 3840x2160 pxixel resolution, and each pixel used 2048 rays - that's **16,986,931,200** rays being simulated! It took multiple hours for my M1 Mac to render these!

## Resources used:
PBRTv4
- https://www.pbrt.org/
- https://github.com/mmp/pbrt-v4

HDRI: 
- created by Greg Zaal on Polyhaven
- provided under the CC0 license
- https://polyhaven.com/a/kloppenheim_02

---

Trackmania Car Model: 
- created by amogusstrikesback2 on Sketchfab
- provided under the CC Attribution license
- https://sketchfab.com/3d-models/trackmania-2020-carsport-c8b80bfc1ed1427eb37f3eba8d1ecfbf

---

Road Texture:
- created by Dmitriy Chugai on texturelib.com
- http://texturelib.com/texture/?path=/Textures/road/road/road_road_0021

--- 

> April 2024