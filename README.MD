#README

* add files xml2json.js and player.js to the target page in order like in the example below

* copy and paste INIT BLOCK

* modify settings
 

```html
<script  src="/xml2json.js"></script>
<script  src="/player.js"></script>
<!-- INIT BLOCK -->
<div id="player"></div>
<script>
  new Ctrl({
   // your video placement tag
    tag: 'https://supply.decenterads.com/?c=v&m=s&placementId=[YOUR PLACEMENT ID]',
    // player run event
    // 'load' - on window load
    // 'timeout' - after timeout
    run: 'load', 
    timeout: 5, // timeout in seconds, required if - run: 'timeout'
    player: {
      ap: true, // auto play video ad
      skipable: true, // is it allowed to skip watching video
      skipAfter: 10, // skip after N seconds
      volume: 0.5, // start volume min - 0, max - 1
      w: 640, // player width
      h: 480 // player height
    }
  })
</script>
<!-- INIT BLOCK END -->
```
