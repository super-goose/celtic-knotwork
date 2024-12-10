# Knotwork

Just a simple doodling application with celtic knotwork.

## To run

From `./` run `http-server` (or whatever static server program you prefer).
It is all static files.

## Purpose

I like the look of celtic knotwork. So I wrote this "application". I have since
been using it as a showcase of my coding style. It is not complex, but it
illustrates a few key points.

### Organization

The part of this project that embodies this concept is the JavaScript code.
(I'll admit, the images all being in the root directory and the JavaScript and
CSS not being in their own fiels are less than ideal.) But the JavaScript code
is structured in a clear way: basic application components defined, logic,
defined, logic connected to UI. There could be other ways to organize it that
make sense too, but the important thing is that the code is grouped. After
looking at it, you know where to find the logic that connects the app logic to
the UI. You know where to find the history and canvas set up.

### Simplicity

Complex projects might call for robust frameworks, but I just wanted to draw
images on an html canvas, where the user touched. So it's one page, with all the
styling and scripting in the same file. And it works. There is no reason to not
use vanilla HTML, CSS and JavaScript here.

### Maintainability

It's important to be able to work quickly on code that you haven't touched in a
while. The code I wrote yesterday, I kind of remember what I was doing. The code
I wrote 2 weeks ago, I don't even remember who wrote it, until git blame points
its finger at me. (Professionally.) (That's a slight exaggeration, but there is
truth in it.)

A few of things that make code easy to refamiliarlize yourself with are plenty
of whitespace, clear variable names, and not playing code golf.

The whitespace allows you recognize shapes and patterns of the code you are
working with. Finding a line of code in 300+ lines of dense text is hard.
Finding a line of code in well-formatted code is much easier.

Clear variable names are the hallmark of self-documenting code. `svBtn` is
probably the save button, but `saveButton` is definitely the save button. The
browser (or compiler or interpreter) doesn't care how long your variable names
are. It only cares that they are not keywords and that they follow the rules of
the language for variable names. So it's important to use the variable names to
tell the engineer what the code is doing.

Not playing code golf... There is no reason to be clever in how you write code.
Cleverness should be reserved for how you solve a problem. If it takes 4 lines
to write something, and someone else can see what it is doing easily, that is
good. If you write 1 line, but it is difficult to figure out what it is doing,
that is bad.

I've tried to employ these philosophies in this project, but as with all
software development, there is inevitably going to be somewhere I've missed the
mark...

### Easy deployment

Having an easy, automated deployment process is very important. Putting assets
in directories was not something I was avoiding, but I think it's telling that
the only thing I bothered to put in a directory was the automated deployment
configuration.
