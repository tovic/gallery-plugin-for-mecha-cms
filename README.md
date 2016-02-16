Gallery Plugin for Mecha CMS
============================

> Image galleries.

Image thumbnails will be generated automatically by the [thumbnail](http://mecha-cms.com/article/thumbnail-plugin "Thumbnail Plugin") plugin where possible, if available.

### Simple Image Gallery

~~~ .no-highlight
{{gallery}}
  [1]: image-1.jpg
  [2]: image-2.jpg
  [3]: image-3.jpg
{{/gallery}}
~~~

### With Image Caption

~~~ .no-highlight
{{gallery}}
  [1]: image-1.jpg "Caption 1"
  [2]: image-2.jpg "Caption 2"
  [3]: image-3.jpg "Caption 3"
{{/gallery}}
~~~

### Manual Thumbnail

~~~ .no-highlight
{{gallery}}
  [1]: image-1.jpg | t-1.jpg "Caption 1"
  [2]: image-2.jpg | t-2.jpg "Caption 2"
  [3]: image-3.jpg | t-3.jpg "Caption 3"
{{/gallery}}
~~~

### Custom Classes

#### Method 1

~~~ .no-highlight
{{gallery.photo.family}}
  [1]: image-1.jpg "Caption 1"
  [2]: image-2.jpg "Caption 2"
  [3]: image-3.jpg "Caption 3"
{{/gallery}}
~~~

Result:

~~~ .html
<div class="p gallery gallery-photo gallery-family">
  <div class="image-group">
    …
  </div>
</div>
~~~

#### Method 2

~~~ .no-highlight
{{gallery class="photo family"}}
  [1]: image-1.jpg "Caption 1"
  [2]: image-2.jpg "Caption 2"
  [3]: image-3.jpg "Caption 3"
{{/gallery}}
~~~

Result:

~~~ .html
<div class="p gallery photo family">
  <div class="image-group">
    …
  </div>
</div>
~~~

### Custom Image Width and Height

~~~ .no-highlight
{{gallery width="200" height="150"}}
  [1]: image-1.jpg "Caption 1"
  [2]: image-2.jpg "Caption 2"
  [3]: image-3.jpg "Caption 3"
{{/gallery}}
~~~

Other attributes will be treated as normal HTML attributes.