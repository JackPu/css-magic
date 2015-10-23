## same height as width(autofit)

```css
.box{
  position:relative;
  width:30%;
  margin:20px 1.5%;
  padding-top:20%;
  background:#fff;
  box-shadow:0 2px 4px rgba(0,0,0,.2);
  
}

/** or **/
.box{
  position:relative;
  width:30%;
  margin:20px 1.5%;
  background:#fff;
  box-shadow:0 2px 4px rgba(0,0,0,.2);
  
}
.box:before{
  content:'';
  float:left;
  padding-top:100%;
  
}

```

Demo1: http://codepen.io/Jack_Pu/pen/QjQBmz

Demo2: http://codepen.io/Jack_Pu/pen/GpQXOz