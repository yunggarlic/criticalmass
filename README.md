# Tim Ferrari Work Examples to Critical Mass

## Statesmen Podcast Website 
<a href="http://statesmenpodcast.com">statesmenpodcast.com</a>
<br /><br/>

### ![Screen Shot 2021-03-02 at 11 26 01 AM](https://user-images.githubusercontent.com/71295717/109688601-1381c480-7b4a-11eb-9e5e-bfc49b8462c2.png)
> The interactive website for the podcast that explores all fifty states with the five senses of perception.
> Access our collection of 100+ episodes, and sort using the clickable SVG map to find one that peaks your interest.

### Explanation
Frontend: Upon an initial load, the user is presented with the show's full podcastography in a responsive grid and sorted by release date. By clicking a state, or another icon as part of the Map, the user is able to sort episodes by their state, or episode type.

![Screen Shot 2021-03-02 at 11 56 10 AM](https://user-images.githubusercontent.com/71295717/109692557-4af27000-7b4e-11eb-8e49-375aab202faa.png)

Every episode has it's own page that holds links to podcast providers (iTunes, Spotify, etc), and an embedded audio player for listeners to tune in on the page itself.

![Screen Shot 2021-03-02 at 11 56 34 AM](https://user-images.githubusercontent.com/71295717/109692605-59408c00-7b4e-11eb-8408-0f4a1d689d62.png)


Backend: Episodes are pulled in by an Axios request and parsed from the show's RSS feed provided by its hosting provider. Each episode is then cached into a Redis NoSQL database and stored for four hours before being deleted, drastically reducing the load time for subsequent site visitors who request episode information within the time frame (thanks initial load-bearers!).

#### Featured Tech
React, Material-UI, Node, ExpressJS, Redis, Axios

## Aether
https://aether-leo.herokuapp.com/
### <img width="500" alt="Screen Shot 2021-02-16 at 6 18 48 PM" src="https://user-images.githubusercontent.com/71295717/127692310-bf93188e-716c-4857-bc6c-0758f5a9079d.png">

### Explanation 
> https://www.youtube.com/watch?v=bSz9XNJkUdM

- An audio-Visual Music Collaboration Experience Our goal is to create a loosely structured audio visual “jam” space for users to compose and visualize music with a variety of instruments collaboratively in a live session. When collaborative art cannot be made in-person, this application brings people together in a creative environment. This audio visual “jam” space serves as a tool to compose and visualize music with a variety of instruments in a live 3-D session.

#### Featured Tech

Three.js, Tone.js, Socket.io, Firebase/Firestore, React, Redux, Express, Framer/Framer-Motion

## Personal Website
http://timferrari.com
### <img width="1440" alt="Screen Shot 2021-07-30 at 1 07 42 PM" src="https://user-images.githubusercontent.com/71295717/127694339-ef9a1791-3332-4586-b323-a90343285238.png">

### Explanation
This is my software development portfolio website, showcasing my coding work and some of my interests.


This website utilizes React and Threejs and leverages react-three-fiber to create componentized 3D assets and scenes, drastically improving DRY practices. In order to get the camera to move around the space, and for objects to exhibit their movement behavior, I used React-Spring to generate many smooth series of integers which were easily translated into rotations and positions.

For the UI, I attempted to use Material-UI but had trouble finding a workflow that suited me. I don't believe I was using the package efficiently at all. Ultimately my usage of it made the whole project feel laborious, even compared to the 3D animation work that had to be done. 

The backend is straight forward, using Express to spin up a server and deliver static assets.

#### Featured Tech
React, React Spring, three.js, react-three-fiber, Material-UI, Node, ExpressJS
