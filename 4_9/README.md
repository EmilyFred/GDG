# Last push before the final project! 

Congrats! You have gone far and you have done great! We need just few more strengths to finish it strong.
Today, we will be covering few things that you might want to add to your project.

## Video

If you are looking for the way to add a video in your `html` files, then here is how we can do that:

### Iframe

``` html
<iframe width="560" height="315" src="https://www.youtube.com/embed/Wye6mK1OiJ4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

This is the basic way how to do that. If you just go to a YouTube video, click share and click `embed`,
it will give you this code.

### Object

``` html
<object width="425" height="344" data="https://www.youtube.com/embed/Wye6mK1OiJ4"></object>
```
This is also another way how to embed a video into your website

### Embed

``` html
<embed src="https://www.youtube.com/embed/Wye6mK1OiJ4" allowfullscreen="true" width="425" height="344">
```

I believe that this is the most inconvenient script, and I highly suggest avoiding doing this way
since some browsers might not understand it.

However, note that the video has a fixed width and height, and it will not be responsive. To make it responsive, you can wrap it into a container:

``` html
<div style="position:relative; padding-bottom:56.25%; padding-top:30px; height:0; overflow:hidden;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/Wye6mK1OiJ4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen style="position:absolute; top:0; left:0; width:100%; height=100%;></iframe>
</div>
```

## Skills Bar

In your portfolio, you will probably want to add some skills that you know. At this point, it's probably
`HTML`, `CSS`, and `JavaScript`.

Let's start with HTML:

``` html
<p>HTML</p>
<div class="container">
  <div class="skills html">90%</div>
</div>

<p>CSS</p>
<div class="container">
  <div class="skills css">80%</div>
</div>

<p>JavaScript</p>
<div class="container">
  <div class="skills js">65%</div>
</div>

```

Now let's add CSS:
``` css
/* Make sure that padding behaves as expected */
* {box-sizing:border-box}

/* Container for skill bars */
.container {
  width: 100%; /* Full width */
  background-color: #ddd; /* Grey background */
}

.skills {
  text-align: right; /* Right-align text */
  padding: 10px; /* Add some padding */
  color: white; /* White text color */
}

.html {width: 90%; background-color: #4CAF50;} /* Green */
.css {width: 80%; background-color: #2196F3;} /* Blue */
.js {width: 65%; background-color: #f44336;} /* Red */
```

## Contact Forms

Here I provide you with contact forms if you want to add one to your website.


### Standard

Here I provide a very simple contact form.


``` html
<div class="container">  
  <form id="contact" action="" method="post">
    <h3>Colorlib Contact Form</h3>
    <h4>Contact us for custom quote</h4>
    <fieldset>
      <input placeholder="Your name" type="text" tabindex="1" required autofocus>
    </fieldset>
    <fieldset>
      <input placeholder="Your Email Address" type="email" tabindex="2" required>
    </fieldset>
    <fieldset>
      <input placeholder="Your Phone Number (optional)" type="tel" tabindex="3" required>
    </fieldset>
    <fieldset>
      <input placeholder="Your Web Site (optional)" type="url" tabindex="4" required>
    </fieldset>
    <fieldset>
      <textarea placeholder="Type your message here...." tabindex="5" required></textarea>
    </fieldset>
    <fieldset>
      <button name="submit" type="submit" id="contact-submit" data-submit="...Sending">Submit</button>
    </fieldset>
  </form>
</div>
```

``` css
@import url(https://fonts.googleapis.com/css?family=Roboto:400,300,600,400italic);
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-font-smoothing: antialiased;
  -moz-font-smoothing: antialiased;
  -o-font-smoothing: antialiased;
  font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
}

body {
  font-family: "Roboto", Helvetica, Arial, sans-serif;
  font-weight: 100;
  font-size: 12px;
  line-height: 30px;
  color: #777;
  background: #4CAF50;
}

.container {
  max-width: 400px;
  width: 100%;
  margin: 0 auto;
  position: relative;
}

#contact input[type="text"],
#contact input[type="email"],
#contact input[type="tel"],
#contact input[type="url"],
#contact textarea,
#contact button[type="submit"] {
  font: 400 12px/16px "Roboto", Helvetica, Arial, sans-serif;
}

#contact {
  background: #F9F9F9;
  padding: 25px;
  margin: 150px 0;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2), 0 5px 5px 0 rgba(0, 0, 0, 0.24);
}

#contact h3 {
  display: block;
  font-size: 30px;
  font-weight: 300;
  margin-bottom: 10px;
}

#contact h4 {
  margin: 5px 0 15px;
  display: block;
  font-size: 13px;
  font-weight: 400;
}

fieldset {
  border: medium none !important;
  margin: 0 0 10px;
  min-width: 100%;
  padding: 0;
  width: 100%;
}

#contact input[type="text"],
#contact input[type="email"],
#contact input[type="tel"],
#contact input[type="url"],
#contact textarea {
  width: 100%;
  border: 1px solid #ccc;
  background: #FFF;
  margin: 0 0 5px;
  padding: 10px;
}

#contact input[type="text"]:hover,
#contact input[type="email"]:hover,
#contact input[type="tel"]:hover,
#contact input[type="url"]:hover,
#contact textarea:hover {
  -webkit-transition: border-color 0.3s ease-in-out;
  -moz-transition: border-color 0.3s ease-in-out;
  transition: border-color 0.3s ease-in-out;
  border: 1px solid #aaa;
}

#contact textarea {
  height: 100px;
  max-width: 100%;
  resize: none;
}

#contact button[type="submit"] {
  cursor: pointer;
  width: 100%;
  border: none;
  background: #4CAF50;
  color: #FFF;
  margin: 0 0 5px;
  padding: 10px;
  font-size: 15px;
}

#contact button[type="submit"]:hover {
  background: #43A047;
  -webkit-transition: background 0.3s ease-in-out;
  -moz-transition: background 0.3s ease-in-out;
  transition: background-color 0.3s ease-in-out;
}

#contact button[type="submit"]:active {
  box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.5);
}

.copyright {
  text-align: center;
}

#contact input:focus,
#contact textarea:focus {
  outline: 0;
  border: 1px solid #aaa;
}

::-webkit-input-placeholder {
  color: #888;
}

:-moz-placeholder {
  color: #888;
}

::-moz-placeholder {
  color: #888;
}

:-ms-input-placeholder {
  color: #888;
}
```

For more contact forms, you can visit [ColorLib](https://colorlib.com/wp/free-html5-contact-form-templates/) website.