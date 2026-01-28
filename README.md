# Time-When-It-Gets-Loud
By Xu Chenchen
 An interactive audiovisual work that within a regular temporal mechanism, visualises how subjective time stretches during silence and compresses during moments of social and emotional intensity.

## Short Description
Time, When It Gets Loud** is an interactive computational artwork that explores how time is perceived differently during moments of quiet routine and moments of emotional or social intensity. The work visualises time as a continuous, steady flow, while allowing sound—such as speech, laughter, or noise—to interrupt and reshape this flow.
Designed for full-screen viewing on a laptop or as a projected installation, the work uses the computer’s built-in webcam and microphone so the audience can activate it through presence and voice.


## Concept 
This project explores how time is experienced differently in quiet, everyday moments and in moments of emotional or social intensity. When time is wholly our own (walking alone, reading), it can feel slow and stretched; moments shared with others (laughter, excitement, social noise) often feel compressed and fleeting.

In the work, time is represented as a continuous and steady visual flow that progresses over a fixed duration. Sound acts as an interruption to this flow. When sound is present, more visual elements appear: text fragments are generated more frequently, fall faster, and accumulate on the screen. When the environment becomes quiet again, these elements gradually disappear.

Rather than measuring time objectively, the piece focuses on time as something shaped by attention, emotion, and interaction. By linking sound to changes in visual density and movement, the work aims to make subjective time visible—how intensity can feel shorter, while quieter moments feel longer.


##Technology Used
My project comprises three interconnected modules integrating time-based animation, sound input analysis, and live camera capture, all operating within a single real-time loop that responds dynamically to audience interaction.
Module 1: 60-Second Time Waveform 
The system begins with a 60-second cycle representing the steady, continuous flow of everyday time. Using millis(), progress is normalized and mapped via lerp() to control a waveform moving from the bottom to the top of the canvas. Unlike earlier sine- and cosine-based exercises, this linear mapping emphasises duration and irreversible flow rather than cyclical repetition. The waveform is generated with beginShape() and vertex(), with subtle irregularity introduced through simplified frequency spectrum data from p5.FFT, giving visual variation without detailed audio analysis.

Module 2: Microphone-Driven Text Interaction
Sound input is captured via p5.AudioIn() and analysed in real time. When amplitude exceeds a threshold, short text fragments are generated and fall at speeds proportional to the sound level, creating a visual metaphor for moments of heightened emotional or social intensity. A silence detection system clears the text when sound remains below the threshold, reflecting a return to routine temporal flow.

Module 3: Floating Webcam Capture
Webcam input is achieved via createCapture(VIDEO), a method introduced in class as the foundational technique for capturing live input. Unlike static display of the camera feed, here it is treated as a dynamic visual object on the canvas. Its position and scaling are controlled through simple motion logic and sound amplitude, applying previously learned shape animation techniques to the live video input.



## How to Run / Install
*Step-by-step instructions.*

## Requirements
*Tech stack, browser, OS, libs.*

## Screenshots / Media
*Include in-action visuals.*

## Credits / Acknowledgements
*Who made it, references.*
##License
*What license is it made under, if any?* 

## Contact / Links
*GitHub repo link, website, demo URL.*
