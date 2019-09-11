# markdown-it-picture

Render images within a `<picture>` element.

`![alt text](http://your.cdn/original/image.jpg "image title")(http://your.cdn/sm/image.jpg "(min-width:0px)")(http://your.cdn/md/image.jpg "(min-width:640px)")(http://your.cdn/lg/image.jpg "(min-width:1280px)")`

… will convert to …

```HTML
<picture>
  <source
    srcset="http://your.cdn/sm/image.jpg"
    media="(min-width:0px)"
  />
  <source
    srcset="http://your.cdn/md/image.jpg"
    media="(min-width:640px)"
  />
  <source
    srcset="http://your.cdn/lg/image.jpg"
    media="(min-width:1280px)"
  />
  <img
    srcset="http://your.cdn/original/image.jpg"
    alt="alt text"
    title="image title"
  />
</picture>
```
