# Welcome

Hello, and welcome to learning HTML fundamentals.
We will try to cover some of the basic functions today in the meeting and assign a
rather difficult homework to do in order to attain an extremely important skill around
IT area - ability to teach yourself. Let's get started!

## Prerequisites

During the meeting I will show you how to use both Vim (text-editor) and Atom (a professional editor for developers).

If you have Mac, you already have it pre-installed. If you have Windows **AND** downloaded `git bash`
while doing the previous homework, then you also have it installed.

*P.S.* In the meeting I will show two basic commands that almost everyone should know, but in case
you didn't come or missed it, here are:
- Press `Esc` and then write `:wq` - in order to exit the file and save it;
- Press `Esc` and then write `:q!` - in order to exit the file without saving it;

## Lesson 1: Let's talk about HTML

I highly recommend start writing your `.html` files locally on computer
and run them. If you experience any problems, [Thimble](https://thimble.mozilla.org) is a
good source (You can click on `Start a scratch project`).

### Structure

Here is a regular blank HTML document that you would want to create before starting changing anything:

```html
<!DOCTYPE html>
<html>
  <head>
    <title> This is the title of our page</title>
  </head>
  <body>
    <h1>Welcome to this page</h1>
  </body>
</html>
```
Let me explain it line by line:
- `<!DOCTYPE html>` - that means that you show to a web browser that it will be an `html` file;
- `<html>` - is a mandatory tag that shows a web browser that you started running html code;
- `<head>` - that is an interesting one, usually used to include any of the scripts, title of a page,
[etc](https://www.w3schools.com/tags/tag_head.asp);
- `<title>` - that is a title of your page, it will be represented in a tab in your browser;
- `<body>` - that is a tag in which you would want to write everything (including your web page
  structure), [more info](https://www.w3schools.com/tags/tag_body.asp)

Does it make sense? If not, it will make sense later. Do not worry much about it, but please try to
read some of the resources.


### Tables

Tables are fun and interesting way of representation of your information/data.
For instance, we would want to create a table like this:

Name | Favorite Pet
--- | ---
Troy | Dog
Jessica | Cat

Let's think about how we will tackle this issue, shall we?

Well, we have three rows and two columns. Then according to [this](https://html.com/tables/) article,
we would want to use tags `table` to declare the table, `tr` three times to represent our rows, and
`th` with `td` to represent values (Names and Favorite Colors) in the given table.

Think for a second how to do that and try to implement it ...
*P.S. you might want to implement it within `<body>` tag*

If you get stuck, the answer is given in the `table.html` file in this directory.

### Images

For instance, you would want to use an image in your web page. It's very easy:

```html
<img src="url_of_your_image" alt="description of your image if it doesn't load">
```
You can also use a locally stored image, put the name of the image and its path instead of url in `<img>` tag.

## Homework

Alright, we are finally at the homework stage.

Here is what you should do:
*Create a web page that explains something that you are passionate about, that you like.
It needs to have:
- at least one image;
- one link to external source to get more information about what you are talking about;
- a table that represents your top five interests (things that you like to do) and its priority
from 0 to 5;*

For instance, if I were to create that table, I would put something like this:

Interests | priority
--- | ---
Swimming in the pool | 2 - rather unimportant
Climbing indoors | 1 - unimportant
Coding at work | 3 - average
Sleeping | 4 - pretty high
Cooking | 5 - highest

Once you are done with your `HTML` page, upload it to `/homework` folder in this directory by doing fork (if you haven't done so) and then changing it locally on your repository and making a pull request



Here are some of my recommendations to go through:
- [HTML game](https://www.w3schools.com/html/exercise.asp) - highly suggest this game to learn more
about html;
- [Great HTML Game](https://codecombat.com) - this is truly a great game, it's interactive;
- [If you feel lost about html](http://htmldog.com/guides/) - great recap, good tutorials;
- [Go-to site for references](https://html.com) - some of their tutorials are dry but I highly recommend
them if you are curios;
