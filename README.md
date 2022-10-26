# GABEstart - A Simple Responsive Startpage

![Gif](asset/gabestart-demo.gif)

**GABEstart** is a simple, clean startpage which can be used on any device like phone, pad, desktop, etc.

It has dark ([Dracula](https://draculatheme.com/contribute)-est theme) and website links are customizable.

🎉**Plus:** Match *GABEstart* with `Dracula X GABE` theme for [Firefox](https://addons.mozilla.org/en-US/firefox/addon/dracula-x-gabe/) 🦊 and [Vivaldi](https://themes.vivaldi.net/themes/P9Xvx24q7Op) 🎻.

## Customizations

See `config.js` file for customization.

### Last.fm Now Playing widget

You must edit (in `index.html` file) the following strings:

```javascript
<script type="text/javascript">
            /*<![CDATA[*/ $(document).ready(function () {
                $("#lastBox").lastplayed({
                    apikey: "[YOU NEED TO GENERATE YOUR OWN LAST.FM API KEY]",
                    username: "[YOUR LAST.FM USER NAME]",
                    limit: 5,
                    refresh: 30,
                });
                $("#playingInfo").nowplaying({
                    apikey: "[YOUR LAST.FM API KEY]", username: "[YOUR LAST.FM USERNAME]", refresh: 60, notplayingtext: '<p class="playing-not">See recently played tracks on: <a href="https://last.fm/user/[USERNAME]" target="_blank">last.fm/user/[USERNAME]</a></p>'
                })
            }); /*]]>*/
  </script>
```

<em>Advice:</em>

> If you're using an adblocker or script blocker you must give permission to access to https://ws.audioscrobbler.com in your personal filters, otherwise the Last.fm widget can't work properly.

### Colors

In the `style.css` you can set an accent color (global) for `username`, `scrollbar` and `parallax` (`waveforms` decoration). Just change the `--accentColor` with a predefined color variable or standard HTML/CSS code color.

Predefined color availables (all of them according to the `Dracula` color palette):

```javascript
var(--black)    // or #282a36
var(--blue)     // or rgb(98, 114, 164)
var(--green)    // or #50fa7b
var(--orange)   // or #ffb86c
var(--purple)   // or #9580ff
var(--red)      // or #ff5555
var(--white)    // or #f8f8f2
var(--yellow)   // or #f1fa8c
```

## Credits

Thanks to [MrAlpha786](https://github.com/MrAlpha786) for the original [GetStarted](https://github.com/MrAlpha786/getstarted) startpage, [RowanFeely](https://github.com/RowanFeely) for [StarterPage](https://github.com/RowanFeely/StarterPage). [Andy Fitzsimon](https://codepen.io/andyfitz) for [the deep blue (waves)](https://codepen.io/andyfitz/pen/aZrKdV) animation and [LentoLen](https://github.com/LentoLen) for [Suggestions](https://github.com/LentoLen/suggestions) script (testing).

---

[more stuff from [GABEweb @ GitHub](https://gabeweb.github.io)]
