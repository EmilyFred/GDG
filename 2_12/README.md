# Welcome to CSS

CSS (Cascading Style Sheets) is used to style and layout web pages — for example,
to alter the font, color, size and spacing of your content, split it into multiple
columns, or add animations and other decorative features.

I am gonna assume that you did your previous homework with `HTML` and now
have basic understanding of tags. Let's say we have a page
that has `body`, `p` tag, and `h1` tag. Can you guess what is happening here?
```css
body {
  background-color: lightblue;
}

h1 {
  color: white;
  text-align: center;
}

p {
  font-family: verdana;
  font-size: 20px;
}
```
As you can see, CSS is pretty straight forward. We have tag `body` that has
value `background-color` to `lightblue` meaning that EVERYTHING that is in
`body` will be `lightblue`.

ANY text that will be within tag `h1` will have text-color of white and it will
be centered on the web page.

ANY text that will be within tag `p` will have a size of 20 px and will have
a font family of `verdana`. If you are not sure what font family is, make sure to google
it for yourself and if you can't figure it out, make sure to ask me this during next meeting!

## How do we connect CSS with HTML?

Now you may be wondering how can we connect CSS with HTML? Well, that's pretty easy and there
are mostly two main ways:

#### Using `<style>` tag

So we can put the tag inside our html code. In real world, people usually prefer to abstain from it,
but once you are learning, it will be pretty good to use it. Let's say I have a very basic structure:
just a paragraph with the phrase `My first style`. Let's see how we can do that:

```html
<!DOCTYPE html>
<html>
  <head>
    <title> My first CSS adventure </title>
  </head>
  <body>
    <p> My first style </p>
    <style>
    p{
      color: red;
    }
    </style>
</html>
```

Seems fairly easy, right? If not, then look again at the code. We added `style` tag to create a text color.

#### Using a completely different CSS file

This is a more advanced method and we will learn how to do that as well, because we want you to be able to
do great things and do them efficiently.

So you want to include a link to your css file inside html, right? So we will use a tag `link`:

```html
...
<head>
  <link rel="stylesheet" type="text/css" href="name_of_my_file.css">
</head>
...
```
So as you can see, it's fairly easy to do that. There is no need to use tag  `style` anymore.

# Homework

As you can see, this tutorial is a little shorter because the more we learn, the more independent you want to become.
In real software engineering world there is a constant push to learn new things fast and that is what we are practicing.

Our homework will consist of several steps:

### Step 1: Go through tutorial

There is a great [tutorial](https://www.codecademy.com/learn/learn-css) that I highly recommend to anyone. It's free and
easy to do. You don't have to finish it completely but do more than 50% of it due next Tuesday.

It will teach you how to do a better job of how to create web pages that are pretty (that have some sort of style).

### Step 2: Go through exercises

[This](https://www.w3schools.com/css/exercise.asp) is by far the best practice that you can get using your CSS skills.
I highly recommend going through it all (but try to do at least first 8 modules).

### Step 3: Bring life to your project

Remember that last week we had to create an html page of your choice? Well, now try to make it pretty by using at least 5 different rules. Your page should have:

- different text styles (*HINT* `font-family`)
- different (either text or background) colors (*HINT* `background-color` or `color`)
- different text aligns (*HINT* `text-align`)
- different links (have at least two different links) that have different styles ([HINT](https://www.w3schools.com/css/css_link.asp))
- if you decide to have a table, then try to add some design to it ([HINT](https://www.w3schools.com/css/css_table.asp))

At this point, once you are done, create a folder `homework/2_11` in your repository, submit there your `html` file and create
a pull request.

### For the bravest

If you feel super adventurous, you can try to create a fully functioning web page using [templates](https://www.w3schools.com/css/css_templates.asp).
If you decide to do that, I am impressed and I will be 24/7 ready to help you with whatever you need.

---
If you are reading at this point, remind me on meeting 2/19 to show you some cool animations that we can do using CSS. 
