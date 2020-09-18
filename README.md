# [OpenPlayer.js](https://www.openplayerjs.com)

![openplayerjs](https://user-images.githubusercontent.com/910829/46182430-d4c0f380-c299-11e8-89a8-c7554a70b66c.png)

[![NPM](https://nodei.co/npm/openplayerjs.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/openplayerjs/)

[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Support%20OpenPlayerJS%20by%20giving%20the%20project%20a%20start%20at%20&url=https://www.openplayerjs.com&hashtags=openplayerjs,mediaplayer,vpaid,opensourcerocks,streaming)
[![JSDelivr](https://data.jsdelivr.com/v1/package/npm/openplayerjs/badge)](https://www.jsdelivr.com/package/npm/openplayerjs)
   [![Build Status](https://travis-ci.org/openplayerjs/openplayerjs.svg?branch=master)](https://travis-ci.org/openplayerjs/openplayerjs) [![Size](https://img.shields.io/bundlephobia/minzip/openplayerjs/latest?style=flat-square)](https://nodei.co/npm/openplayerjs) [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/rafa8626?locale.x=en_US)

This is a media player that uses all the goods of HTML5 video/audio elements to play the most popular media in MP4/MP3, HLS and M(PEG)-DASH, and also has the ability to play VMAP, VAST and VPAID ads.

## Advantages

* Supports **IE11+ (Win8) and all modern browsers**.
* No dependencies, since it is written in Typescript.
* Runs a simple but yet powerful algorithm to **check the browser's autoplay capabilities** across browsers.
* Supports for **local and remote captions** for **both video and audio**, even without including the `crossorigin` attribute.
* **Enhance your player** adding your own buttons. Check [here](./docs/add-custom.md) for more details.
* Provides the ability to use a single VAST/VPAID source or a VAST/VPAID playlist from several different sources (including URLs and valid XML strings).
* **Can play ads in infinite loop**, desired for ads that are in a heavy text page.
* Always **responsive** by default, for both video/audio tags; a new **`fill`** mode is also included to scale and crop media relative to its parent container.

## Getting Started

```html
<html>
    <head>
        <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.css">
    </head>
    <body>
        <video class="op-player__media" id="player" controls playsinline>
            <source src="/path/to/video.mp4" type="video/mp4">
            <track kind="subtitles" src="/path/to/video.vtt" srclang="en" label="English">
        </video>
        <script src="https://cdn.jsdelivr.net/npm/openplayerjs@latest/dist/openplayer.min.js"></script>
        <script>
            // Check the `API and events` link below for more options
            const player = new OpenPlayer('player');
            player.init();
        </script>
    </body>
</html>
```

## Usage and API Guides

If you want to unleash the power of OpenPlayerJS, check the following links to learn how to customize it.

* [Advanced use](./docs/usage.md)
* [API and events](./docs/api.md)
* [How to add custom controls/players](./docs/customize.md)

## Code Samples

1. [No configuration (only DOM classes)](https://codepen.io/rafa8626/pen/WaNxNB)
2. [Minimal configuration](https://codepen.io/rafa8626/pen/BqazxX)
3. [Using `fill` mode](https://codepen.io/rafa8626/pen/xxZXQoO)
4. [Using Ads](https://codepen.io/rafa8626/pen/vVYKav)
5. [Removing controls and using `preload="none"`](https://codepen.io/rafa8626/pen/OJyMwxX)
6. [Add source after initialization (useful for AJAX)](https://codepen.io/rafa8626/pen/YzzgJrK)
7. [Using `Levels`](https://codepen.io/rafa8626/pen/ExxXvZx)
8. [Playing HLS streaming with DRM (Encryption)](https://codepen.io/rafa8626/pen/QZWEVy)
9. [M(PEG)-DASH with Ads](https://codepen.io/rafa8626/pen/Xxjmra)
10. [Basic playlist (video and audio)](https://codepen.io/rafa8626/pen/GRREQpX)
11. [Ads playlist (multiple URLs)](https://codepen.io/rafa8626/pen/wvvxbMN)
12. [Retrieve data from audio streaming (HLS)](https://codepen.io/rafa8626/pen/abbjrBW)
13. [YouTube video (using plugin)](https://codepen.io/rafa8626/pen/wvvOYpg)
14. [Addition of a custom control](https://codepen.io/rafa8626/pen/oNXmEza)
15. [OpenPlayerJS with Next.js](https://codesandbox.io/s/vigorous-almeida-71gln)
16. [Using hls.js p2p plugin](https://codepen.io/rafa8626/pen/PoPLMxo)

## Built With

* [Typescript](https://www.typescriptlang.org/docs/home.html) - The Javascript for Pros.

## Authors

* **Rafael Miranda** - [rafa8626](https://github.com/rafa8626)

See also the list of [contributors](https://github.com/openplayerjs/openplayerjs/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
