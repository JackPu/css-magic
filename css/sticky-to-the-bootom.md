# Sticky To The Bottom

we always want to make a footer sticky to the bottom of the page and we don't need to care about the height of the page.

Let's see [demo](http://codepen.io/Jack_Pu/pen/zvdmzv) 

## css

```css
/* Mostly: http://ryanfait.com/sticky-footer/ */

* {
	margin: 0;
}
html, body {
	height: 100%;
}
.page-wrap {
  min-height: 100%;
  /* equal to footer height */
    margin-bottom: -60px; 
}
.page-wrap:after {
  content: "";
  display: block;
}
.site-footer, .page-wrap:after {
	height: 60px;
  line-height:60px;
}
.site-footer {
  background: #1ba1e2;
  text-align:center;
}
.site-footer a{
  
  color:#fff;
}

```

## html

```html

<div class="page-wrap">
  
  <h1>Sticky To The Bottom</h1>
     
</div>

<footer class="site-footer">
  <a href="">my Github</a>
</footer>


```
