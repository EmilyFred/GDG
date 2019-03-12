# Making things prettier

You survived the mid-project. Congratulations! It's been a hard one but today we will start learning something that is
most people use in their day-to-day world - Bootstrap!

## What is it?

It's a framework that helps you to create pretty objects easier and faster. How? You know that if we want to create
an object, let's say, a table, it will have its own padding and border the way you want it based on its CSS.
Bootstrap has those objects already written down so you can import those objects directly rather than
creating something from scratch.

## How?

Alright, this one is pretty important. You have two options of enabling it:
- via a source script in your HTML head or;
- via importing those files directly to your local machine (laptop).

The one that I recommend is just creating a source script link inside your html.

### Steps

1) Go to the [website](https://getbootstrap.com/)
2) Copy paste the link into your HTML file
3) Read documentation and try to create some objects

Here is an example:
``` html
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

Try it for yourself!

## Homework

1) Create a web page that will use Bootstrap and have **ALL** of the following:
- Buttons
- Card
- Dropdown
- Media object
- Popover
- Spinner (*This one is optional*)

2) Watch the whole course of the [following](https://scrimba.com/g/gbootstrap4)

It should not take you more than 1 hour but will significantly improve your understanding of Bootstrap.

3) FOR THE BRAVEST

There is `index.html` in the directory. It looks bad and crooked intentionally. Try to fix the code to make it look better.

### Submission instruction

Submit your `html` file in the format of your name_date. In this case, I would submit it as `aleksandr_3_12.html`. Make a pull request and I will take a look.
