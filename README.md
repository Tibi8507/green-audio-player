# Green Audio Player

Based on a [pen](https://codepen.io/gregh/pen/NdVvbm) I've created 2 years ago.
Due to requests from many people I decided to create a repository, 
containing an improved version of the Green Audio Player including the support for multiple audio players on a single page.

#### [Online demo](https://codepen.io/gregh/full/NdVvbm)

## Usage

Include the `green-audio-player.css` or `green-audio-player.min.css` file:

```html
<link rel="stylesheet" type="text/css" href="{path}/dist/css/green-audio-player.min.css">
```
and `green-audio-player.js` file (or `green-audio-player.min.js`): 
```html
<script src="{path}/dist/js/green-audio-player.js"></script>
```

Alternatively, you can load it from CDN:

```html
<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/gh/greghub/green-audio-player/dist/css/main.min.css">
<script src="https://cdn.jsdelivr.net/gh/greghub/green-audio-player/dist/js/green-audio-player.min.js"></script>
```

Add the audio tag inside of a container. You are free to add any attributes.
Green Audio Player does not change the audio tag, so for example if you want the audio to loop,
you can add the loop attribute to the audio tag.

```html
<div class="gap-example">
    <audio>
        <source src="audio/example-1.mp3" type="audio/mpeg">
    </audio>
</div>
```

This will initialize the Green Audio Player
```javascript
new GreenAudioPlayer('.gap-example');
```

You can add multiple players on a single page.
Refer to `/examples` folder for demos of single and multiple players.
