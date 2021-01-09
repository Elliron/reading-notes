# Images

Create classes for ease when dealing with images.
image sizes such as small medium and large.  

```
img.small {
  width: 100px;
  height: 100px;
}

```

Classes for aligning such as left and right

```
img.align-leftg {
  float :left;
  margin-right: 10px;
}
```

Centering images

```
img.align-center {
  display block;
  margin: 0px auto;
}
```

background images

```
body {
  background: color imageUrl repeat attachment position
}
```

# Practical Information

Search Engine Optimization or SEO can help visitors find your sight
By entering keywords into titles, alt tags, headings and throughout your page it can bump your site up the search engine list.  Search Engines are smart, they can tell when they are being manipulated and may penalize you.  Keywords should be things that your target audience will search for, narrowing it down by location for example may help your target customers find your site.  There are tools online that you can use to track the user data of your visitors and better adjust to their needs.

# Video and Audio API's

```
<div class="player">
  <video controls>
    <source src="linkToVideo.mp4" type="video/mp4>
    <source src ="linkToVideoAlt.webm" type="video/webm>

    </video>
    <div class="controls">
    <button class="play" data-icon="P" aria-label="play pause toggle"></button>
    <button class ="stop" data-icon="S" aria-label="stop></button>
    <div class="timer">
    <div></div>
    <span aria-label="timer">00:00</span>
    </div>
    <button class="rwd" data-icon="B" aria-label="rewind"></button>
    <button class="fwd" data-icon="F" aria-label="fast forward"></button>
    </div>
    </div>
```

When creating your own video and audio controls ensure that the previous button is canceled before the new one starts.  I.e. do not allow the rewind and fast forward button to be enabled at the same time



[Home](../README.md)