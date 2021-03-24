# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Marshall Blatz**

Time spent: **5** hours spent in total

Link to project: [bow-woolly-responsibility](https://glitch.com/edit/#!/bow-woolly-responsibility)

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [X] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [X] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:

![](https://cdn.glitch.com/f6a12758-3c8f-401c-93ce-268b3e3eecf6%2Fezgif.com-gif-maker.gif?v=1616542696901)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.
 
To complete the required parts of this assignment, I didn't need any 
outside resources. In order to randomize patterns I used [stack overflow](https://stackoverflow.com/questions/4550505/getting-a-random-value-from-a-javascript-array).
To get pictures for the buttons, I used [unsplash](https://unsplash.com/).
I used [w3 schools](https://www.w3schools.com/css/css_align.asp) to help me with centering the images within the buttons.


2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 

A challenge I encountered when creating this submission was getting the images of animals to appear over the buttons when the user clicked them. I haven’t had much experience with traditional CSS before this project, so it was good practice. My first issue was that I couldn’t pull the images from the assets folder using src=”assets/example-name.jpg” syntax. I found a way around this by going to the assets folder and using the generated links that glitch created for each asset. The next problem I had with this task was making the images fit the button perfectly. I did a lot of trial and error using different CSS properties to adjust the margins, width, and height of the images. In the end, manually adjusting the margins was the best fix I found. W3schools.com was really helpful with explaining to me how different CSS properties can be used to help align objects within containers.

Another challenge that I encountered was finding a way to randomize the pattern each game. I decided to make a function that took an array as input. I wasn’t sure if arrays were pass-by-reference in Javascript, but I knew they were in Java so I tested to see if they were. I changed a value in the pattern array within the randomize function and sure enough, the array changed outside of the function. Knowing this, I knew I didn’t have to return any values from my new function. The next step in randomizing was to loop through the whole array and assign random values within a range to each index. Again, I knew how to do this in Java, but not Javascript so I checked stack overflow to see if it worked the same, and it pretty much did. After this, I just implemented Math.floor(Math.random(......)) and called the function at the start of the game which ended up working.


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words)

After completing this project, I feel like I learned a lot and came to realize how much work needs to go into something that looks seemingly simple. A question that I have now is how would one build a multi-page website? Would there be one root page linked to all the rest? Does there need to be one stylesheet and script per page? I also started to wonder about how my favorite websites worked. How does a developer implement a system in which users can create an account, leave the site, and have all their information saved? Where does a developer store all this information? How do they make it secure enough for users to trust them?


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

If I had a few more hours, I would finish adding sounds to the project. I had an idea from the start of making every button a different farm animal, and having all the sounds be animal sounds. I thought this would make it a better game for little kids so they could improve their memory skills while learning about animals. I ended up downloading sounds for this and I even imported them into the glitch file, but I didn’t have enough time in my schedule to find a way to implement them. I also think adding a feature in which the game keeps adding onto the pattern until the user fails would be cool. They would then get a score at the end of the game representing how many levels they got past.



## License

    Copyright Marshall Blatz

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
