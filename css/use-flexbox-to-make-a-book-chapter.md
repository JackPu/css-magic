#use Flexbox to make a book chapter

you can see demo [here](http://codepen.io/Jack_Pu/pen/yyqzWp) 


###html

```html
<h5>Naruto</h5>
<ul class="list">
    <li class="hbox"><a href="#">As a Taijutsu User</a><span class="spacer boxFlex"></span><span class="sect"> 601</span></li>
   <li class="hbox"><a href="#">The Night Before the Second Exam</a><span class="spacer boxFlex"></span><span class="sect"> 602</span></li>
   <li class="hbox"><a href="#">The Three Questions</a><span class="spacer boxFlex"></span><span class="sect"> 603</span></li>
   <li class="hbox"><a href="#">The New Chunin Exams</a><span class="spacer boxFlex"></span><span class="sect"> 604</span></li> 
  <li class="hbox"><a href="#">The Hidden Heart</a><span class="spacer boxFlex"></span><span class="sect"> 605</span></li>
  <li class="hbox"><a href="#">Hanabi's Decision</a><span class="spacer boxFlex"></span><span class="sect"> 605</span></li>
  <li class="hbox"><a href="#">My First Friend</a><span class="spacer boxFlex"></span><span class="sect"> 605</span></li>
  
    
</ul>

```

### css

```html

.list{
  position:relative;
  width:720px;
  margin:60px auto;
}


/** just view here **/
.hbox {
    display: -webkit-box;
    -webkit-box-orient: horizontal;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: horizontal;
    -moz-box-align: stretch;
    display: box;
    box-orient: horizontal;
    box-align: stretch;
    width: 100%;
    margin-top: 15px;
}

.hbox > * {
    -webkit-box-flex: 0;
    -moz-box-flex: 0;
    box-flex: 0;
    display: block;
}

span.spacer {
    color: #2e87dd;
    margin: 0 3px 0 5px;
    background-image: url(http://blog.freleap.com/events/svg/static/img/dot.png)   ;
    background-repeat: repeat-x;
    background-position: left 13px;
}

 .boxFlex {
    -webkit-box-flex: 1;
    -moz-box-flex: 1;
    box-flex: 1;
 }

```