# GABEstart - A Simple Responsive Startpage

![Gif](asset/gabestart-demo.gif)

**GABEstart** is a simple, clean startpage which can be used on any device like phone, pad, desktop, etc.

It has dark ([Dracula](https://draculatheme.com/contribute)-est theme) and light mode. And website links are customizable.

## Customizations

See `config.js` file for customization.

### Last.fm Now Playing widget

You must edit (in `index.html` file) the following strings:

```html
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

## Credits

Thanks to [MrAlpha786](https://github.com/MrAlpha786) for the original [GetStarted](https://github.com/MrAlpha786/getstarted) startpage and [RowanFeely](https://github.com/RowanFeely) for [StarterPage](https://github.com/RowanFeely/StarterPage).
