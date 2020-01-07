# Javascript Webcam

Wes Bos Youtube Tutorial: [Unreal Webcam Fun with getUserMedia() and HTML5 Canvas - #JavaScript30 19/30](https://www.youtube.com/watch?v=ElWFcBlVk-o&list=PLu8EoSxDXHP6CGK4YVJhL_VWetA865GOH&index=19).

*** Note: to open web links in a new window use: _ctrl+click on link_**

## Table of contents

* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Features](#features)
* [Status](#status)
* [Inspiration](#inspiration)
* [Contact](#contact)

## General info

* Tutorial Code for a webcam in javascript app, using a local server to host the webcam.

## Screenshots

![Example screenshot](./img/webcam.png).
![Example screenshot](./img/server.png).

## Technologies

* Ran in Google Chrome browser with: [Javascript engine V8 7.9.317.32 for Windows (x64)](https://v8.dev/).

## Setup

* run 'npm i' to install 'browser-sync' package then type 'npm run'.

## Code Examples

* function to get video stream data and play it.

```javascript
function getVideo() {
  navigator.mediaDevices.getUserMedia({ video: true, audio_: false })
  .then(localMediaStream => {
    console.log(localMediaStream);
    video.srcObject = localMediaStream;
    video.play();
  })
  .catch(err => {
    console.error(`oh no!!`, err);
  });
}
```

## Features

*  Updated as video.src is deprecated in Chrome Browser: video.srcObject is the new version.

## Status & To-Do List

* Status: Working.

* To-Do: fix filters code - filtering not working well.

## Inspiration

* Wes Bos Youtube Tutorial: [Unreal Webcam Fun with getUserMedia() and HTML5 Canvas - #JavaScript30 19/30](https://www.youtube.com/watch?v=ElWFcBlVk-o&list=PLu8EoSxDXHP6CGK4YVJhL_VWetA865GOH&index=19).

## Contact

Repo created by [ABateman](https://www.andrewbateman.org) - feel free to contact me!