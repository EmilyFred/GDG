# Welcome back

Alrighty, you have made it this far! Great! Few things to touch on:

- `HTML5` and `Arduino` are not added since I have not received a response from anyone who wanted to pursue those routes;

 Now, at this point you should feel comfortable with Bootstrap, right?

 Let's create a Bootstrap template:

 ```html
 <!DOCTYPE html>
 <head>
   <title> My title name </title>
   <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
 </head>
 <body>
 <!-- Let's create some things here -->
 <div class="alert alert-info" role="alert">
   A simple info alert—check it out!
 </div>
 </body>
 </html>
 ```

## Elements

Let's look at different elements that we can create! Copy paste from here to your code and see for yourself!

### Borders

We could change their colors and shape:

``` html
<span class="border border-primary"></span>
<span class="border border-secondary"></span>
<span class="border border-success"></span>
<span class="border border-danger"></span>
<span class="border border-warning"></span>
<span class="border border-info"></span>
<span class="border border-light"></span>
<span class="border border-dark"></span>
<span class="border border-white"></span>
<!-- Images below with different shapes -->
<img src="..." alt="..." class="rounded mb-0">
<img src="..." alt="..." class="rounded-top">
<img src="..." alt="..." class="rounded-right">
<img src="..." alt="..." class="rounded-bottom">
<img src="..." alt="..." class="rounded-left">
<img src="..." alt="..." class="rounded-circle">
<img src="..." alt="..." class="rounded-pill">
<img src="..." alt="..." class="rounded-0">
```

### Fonts

We can create different types of font weights

``` html
<p class="font-weight-bold">Bold text.</p>
<p class="font-weight-bolder">Bolder weight text (relative to the parent element).</p>
<p class="font-weight-normal">Normal weight text.</p>
<p class="font-weight-light">Light weight text.</p>
<p class="font-weight-lighter">Lighter weight text (relative to the parent element).</p>
<p class="font-italic">Italic text.</p>
```


### Buttons

We can make various buttons
``` html
<button type="button" class="btn btn-primary">Primary</button>
<button type="button" class="btn btn-secondary">Secondary</button>
<button type="button" class="btn btn-success">Success</button>
<button type="button" class="btn btn-danger">Danger</button>
<button type="button" class="btn btn-warning">Warning</button>
<button type="button" class="btn btn-info">Info</button>
<button type="button" class="btn btn-light">Light</button>
<button type="button" class="btn btn-dark">Dark</button>
<button type="button" class="btn btn-link">Link</button>
```

We can also make gradient buttons

``` html
<button class="btn peach-gradient">Peach</button>
<button class="btn purple-gradient">Purple</button>
<button class="btn blue-gradient">Blue</button>
<button class="btn aqua-gradient">Aqua</button>
```

Outline buttons:
``` html
<button type="button" class="btn btn-outline-primary waves-effect">Primary</button>
<button type="button" class="btn btn-outline-default waves-effect">Default</button>
<button type="button" class="btn btn-outline-secondary waves-effect">Secondary</button>
<button type="button" class="btn btn-outline-success waves-effect">Success</button>
<button type="button" class="btn btn-outline-info waves-effect">Info</button>
<button type="button" class="btn btn-outline-warning waves-effect">Warning</button>
<button type="button" class="btn btn-outline-danger waves-effect">Danger</button>
```

Floating buttons

``` html
<a class="btn-floating btn-lg purple-gradient"><i class="fas fa-bolt"></i></a>
<a class="btn-floating peach-gradient"><i class="fas fa-leaf"></i></a>
<a class="btn-floating btn-sm blue-gradient"><i class="fas fa-star"></i></a>
```

Buttons with icons

``` html
<button class="btn btn-primary"><i class="fas fa-magic mr-1"></i> Left</button>
<button class="btn btn-default">Right <i class="fas fa-magic ml-1"></i></button>
```

Social buttons

``` html
<!--Facebook-->
<button type="button" class="btn btn-fb"><i class="fab fa-facebook-f pr-1"></i> Facebook</button>
<!--Twitter-->
<button type="button" class="btn btn-tw"><i class="fab fa-twitter pr-1"></i> Twitter</button>
<!--Google +-->
<button type="button" class="btn btn-gplus"><i class="fab fa-google-plus-g pr-1"></i> Google +</button>
<!--Linkedin-->
<button type="button" class="btn btn-li"><i class="fab fa-linkedin-in pr-1"></i> Linkedin</button>
<!--Instagram-->
<button type="button" class="btn btn-ins"><i class="fab fa-instagram pr-1"></i> Instagram</button>
<!--Pinterest-->
<button type="button" class="btn btn-pin"><i class="fab fa-pinterest pr-1"></i> Pinterest</button>
<!--Vkontakte-->
<button type="button" class="btn btn-vk"><i class="fab fa-vk pr-1"></i> Vkontakte</button>
<!--Stack Overflow-->
<button type="button" class="btn btn-so"><i class="fab fa-stack-overflow pr-1"></i> Stack Overflow</button>
<!--Youtube-->
<button type="button" class="btn btn-yt"><i class="fab fa-youtube pr-1"></i> Youtube</button>
<!--Slack-->
<button type="button" class="btn btn-slack"><i class="fab fa-slack-hash pr-1"></i> Slack</button>
<!--Github-->
<button type="button" class="btn btn-git"><i class="fab fa-github pr-1"></i> Github</button>
<!--Comments-->
<button type="button" class="btn btn-comm"><i class="fas fa-comments pr-1"></i> Comments</button>
<!--Email-->
<button type="button" class="btn btn-email"><i class="fas fa-envelope pr-1"></i> Email</button>
<!--Dribbble-->
<button type="button" class="btn btn-dribbble"><i class="fab fa-dribbble pr-1"></i> Dribbble</button>
<!--Reddit-->
<button type="button" class="btn btn-reddit"><i class="fab fa-reddit-alien pr-1"></i> Reddit</button>
```

# Homework

## Step 1: Make sure that you are aware of this website

This [website](https://mdbootstrap.com) is **VERY** useful to refer yourself to Bootstrap.


## Step 2: Create your own landing page

You have an image in this repository. Try to create a web page out of this picture. It's about the frozen yogurt.

Here are some requirements:
- You have social media links (*you don't need to have an actual link leading to something, `href` doesn't matter*)
- You have **at least** 3 pictures on the web page
- The greenish-yellowish line **must** represent 4 different buttons (*again, they don't need to lead anywhere specifically*)

That's all! This Homework should be quite complicated for you but let me know if you get stuck.
Remind me to show you a solution to the website next time.
