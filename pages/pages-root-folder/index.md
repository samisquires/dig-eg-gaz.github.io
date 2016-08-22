---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "Blog"
  url: 'http://dig-eg-gaz.github.io/blog/'
  image: logo.jpg
  text: 'Reflections on the content of the <em>Egyptian Gazette</em>, and the work of digitization. Authored by the students in IFS 2116.'
widget2:
  title: "Instructions"
  url: 'http://dig-eg-gaz.github.io/how-to/'
  text: 'How to do all this stuff...'
  video: '<iframe width="560" height="315" src="https://www.youtube.com/embed/n0FEV3pwRII" frameborder="0" allowfullscreen></iframe>'
widget3:
  title: "Contents"
  url: 'http://dig-eg-gaz.github.io/contents/'
  image: logo.jpg
  text: 'Full text of the paper will slowly unroll here.'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: https://tinyletter.com/feeling-responsive
  text: Inform me about new updates and features ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
