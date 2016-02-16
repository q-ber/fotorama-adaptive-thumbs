# fotorama-plugin

This Jquery plugin makes fotorama (fotorama.io) slider thumbnails adaptive for different screen sizes in real time. 

Before use this plugin, you need include into your project jquery-lib (1.9.0) or newer and fotorama plugin (http://fotorama.io/)
```
<script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"></script>
<script type="text/javascript" src="./js/fotorama.js"></script>
```

Then you need to include fotorama adaptive thumbnails plugin and initialize it
```
<script type="text/javascript" src="./js/fotoramaAdaptiveThumbs.js"></script>
<script type="text/javascript">
  jQuery(document).ready(function($) {
    $(".fotorama").autoThumbs({
      'number': 'auto',
      'width' : '100%',
      'ratio' : '16:9'
    });
  });
</script>
```

## variables

**number** - the number of thumbnails that will be displayed in the scope. It may be *'auto'* - default value, plugin count number of thumbnails and try to contain them into the scope or *(int) Number* - simple number.

**width** - width of viewport. It may be *'auto'* - default value, *X%* - in percents, *X* - in pixel

**ration** - ratio between width and height of thumbnail. It maybe like *16:9* or *4:3* or something else in similar rules, or may be *1.33333* 
