# Welcome to JavaScript

Welcome to JavaScript - a language that is used in many fields of Computer Science.
You can build a lot of different things but we will look into Web Development aspect of it only today.

## Why use JavaScript?

Well, imagine you have a fancy looking sign up or registration form, at this point you have some idea on how to create it
and possibly a good skill in making it pretty but probably no functionality. What it means is that your form
just exists but doesn't do anything. That's where we would want to use JavaScript.

Let me show you an example of creating a Contact form

### Example: Contact form

Of course, we need to start with the HTML code first. Let's use tags `div` to logically separate two blocks:

```html
<!DOCTYPE html>
<html>
  <head>
    <title> Contact form using JS </title>
  </head>
  <body>
    # let's have a tag main and a tag form
      <div id="main">
        <h1> Contact form using JS</h1>
        <div id="form"></div>
      </div>  
  </body>
</html>
```

So far, that's enough. It doesn't show much prettiness - in fact all we can see now is just a paragraph text.

Now, let's add some `JavaScript`
``` javascript
var x = document.getElementById("form");
var createForm = document.createElement("form"); // now we are creating a new element form
createForm.setAttribute("action", ""); // we are setting action attribute
createForm.setAttribute("method", "post"); // setting method attribute
x.appendChild(createForm);

var heading = document.createElement("h2");
heading.innerHTML = "Contact Form";
createForm.appendChild(heading)

var line = document.createElement("hr");
createForm.appendChild(line);

var linebreak = document.createElement("br");
createForm.appendChild(linebreak);

var namelabel = document.createElement("label");
namelabel.innerHTML = "Your name : ";
createForm.appendChild(namelabel);


var inputelement = document.createElement('input'); // Create Input Field for Name
inputelement.setAttribute("type", "text");
inputelement.setAttribute("name", "dname");
createForm.appendChild(inputelement);

var linebreak = document.createElement('br');
createForm.appendChild(linebreak);

var emaillabel = document.createElement('label'); // Create Label for E-mail Field
emaillabel.innerHTML = "Your Email : ";
createForm.appendChild(emaillabel);

var emailelement = document.createElement('input'); // Create Input Field for E-mail
emailelement.setAttribute("type", "text");
emailelement.setAttribute("name", "demail");
createForm.appendChild(emailelement);

var emailbreak = document.createElement('br');
createForm.appendChild(emailbreak);

var messagelabel = document.createElement('label'); // Append Textarea
messagelabel.innerHTML = "Your Message : ";
createForm.appendChild(messagelabel);

var texareaelement = document.createElement('textarea');
texareaelement.setAttribute("name", "dmessage");
createForm.appendChild(texareaelement);

var messagebreak = document.createElement('br');
createForm.appendChild(messagebreak);

var submitelement = document.createElement('input'); // Append Submit Button
submitelement.setAttribute("type", "submit");
submitelement.setAttribute("name", "dsubmit");
submitelement.setAttribute("value", "Submit");
createForm.appendChild(submitelement);

```

Now, that's a lot of code!!! But don't get too overwhelmed by it! It will make sense once you get to work with it more.

Now, let's think about Styling:

``` css

/* Below line is write to use Google font online */
@import "http://fonts.googleapis.com/css?family=Ubuntu";
div#main{
width:830px;
height:650px;
margin:0 auto;
font-family:'Ubuntu',sans-serif
}
div#form{
text-align:center;
border:1px solid #ccc;
width:300px;
padding:0 50px 15px;
margin-top:20px;
box-shadow:0 0 15px;
border-radius:6px;
float:left
}
#main h1{
margin-top:40px
}
hr{
margin-top:-5px
}
label{
float:left;
font-size:16px
}
input[type="text"]{
width:100%;
margin-top:10px;
height:35px;
margin-bottom:25px;
padding:10px;
border:3px solid #2BC1F2
}
textarea{
width:100%;
border:3px solid #2BC1F2;
padding:10px;
margin-bottom:25px;
margin-top:10px;
height:100px;
resize:none
}
input[type="submit"]{
width:100%;
padding:10px 45px;
background-color:#2BC1F2;
border:none;
color:#fff;
font-size:18px;
font-weight:700;
cursor:pointer;
font-family:'Ubuntu',sans-serif
}
```
Now it may make you confused. However, I encourage you to try to understand it and if you have any problems understanding it, try googling on how to create a contact form.


## Homework

Now this homework will be not as difficult as it was before since it's better to feel and play around with JavaScript for awhile.

### Step 1: Contact Form

This one is very simple! Try following [this](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Your_first_HTML_form) tutorial. It's pretty straightforward and you
will learn how to create a simple form.

**However**, if you are struggling with that one, here are couple videos that you are free to follow:
- [HTML,CSS+JS](https://www.youtube.com/watch?v=GAOBXGPuKqo) - pretty short video with explanations;
- [Form](https://www.youtube.com/watch?v=mJa_3IiKxFk) - even shorter video still easy to follow;
- [Extensive](https://www.youtube.com/watch?v=7BlmTHjIk24) - really extensive video and easy to follow, pretty long but I highly recommend following exactly this one;

### Step 2: Try to create a simple calculator

Feel free to use any resources: Internet, books, GitHub to find any information on how to create a simple calculator. It could do whatever:
- you can make it to be able to only add two numbers together (the easiest option);
- you can make it do all possible variations along with drawing graphs (the hardest option);

As a suggestion resource, I suggest [this](https://www.youtube.com/watch?v=opz_-qeDi2E&list=PLLAZ4kZ9dFpPQbcrA-SzALJeFm23tPrAI&index=10) one.

### Step 3: PLAY GAMES :)

I am not kidding, try to play [CodeAcademy](https://www.codecademy.com/learn/introduction-to-javascript). It's a great source to learn JavaScript.
I don't know any other game that could teach you better JavaScript.

## Resources to learn

- [JavaScript for cats](http://jsforcats.com) - a great source for learning JavaScript, extremely simple and yet thorough;
- [Screeps](https://screeps.com) - a pretty difficult yet intriguing game to learn JavaScript;
- [CodeCombat](https://codecombat.com) - already advertised but still a great game for learning;
- [Mozilla Learn](https://developer.mozilla.org/en-US/docs/Web/JavaScript) - a little bit advanced documentation on JavaScript, but I highly
recommend doing it in the future
- [CheckIO](https://checkio.org) - a really interesting game to learn JavaScript
- [CodeAcademy](https://www.codecademy.com/learn/introduction-to-javascript) - of course, I highly recommend CodeAcademy for learning purposes;
- [Learn-JS](https://www.learn-js.org) - a website made specifically for learning JavaScript
