# A Basic Project
\label{cha:chapter-1-basic-project}

Welcome to [A Jekyll Book: Web Development for Mad Scientists](http://linktojekyllbook/). Our purpose in this book is to begin the journey toward web devevelopment mastery. The journey of a thousand sites begins with a single commit. (Footnote: everone else has misqouted Lao-tzu, I'm going to as well. [http://www.quotationspage.com/quote/24004.html](http://www.quotationspage.com/quote/24004.html))

We will begin this journey with our trusted blade: [Jekyll](http://jekyllrb.com/). Jekyll is a "static site generator", a new trend in web design that favors lightweight, pre-assembled websites over heavy, dynamic "content management systems".

If you are unfamiliar with any of these concepts, fear not. We will walk through the steps in detail. On our way to building (yet another) Jekyll template "alterego", we will learn basic web technologies, HTML5, CSS, JavaScript, version control, and deployment. Experienced web developers will quicky introduce you to the world of static generation and help explore the power thousands of developers have been discovering over the course of the last few years.

A Jekyll Book takes a holistic approach to web development by building a real-world example website. Although *I* will be building the afrementioned "alterego" template, I encourage *you* to build what every aspiring 21st Century Web Developer needs: a personal brand portfolio site. (We will templatize the code beneath your website so that it is easy to fork as a starting point for additional sites you'll be itching to build. And since you'll no doubt be an expert after this book, we look forward to posting your success story--and pictures of you swimming in your coin vault--on our website.)

This first chapter will introduce you to the mind-like-water status with a quick demo of the default Jekyll template. In a matter of minutes, we'll create an initial personal blog template, place it under version control (git), and deploy it to the public (via GitHub).

In Chapter 2, we'll start from scratch, but implement a more sophisticated project instance. We will learn how to build a custom Cloud based development environment, capable of handling multiple versions of Jekyll's runtime simultaneously. We will learn an easy way to keep your envorinment sync'd with GitHub Pages.

The rest of the book will branch out and explore standard (and a few more obscure) features of modern websites. We will, of course, investigate how to utilize the strengths of Jekyll to assist in implementation details.

## Introduction
\label{sec:introduction}

What is Jekyll anyway, and why would I want to use it to write websites?

### Prerequisites

### Conventions

## On Cloud 9

(Footnote: It's very difficult for me to resist puns, folks. I really don't even try anymore.)

Cloud 9 is a cloud development environment. A combiation of an Ubuntu server, specialized for development, with a web-based Integrated Development Environment front-end.

You can spin up various workspaces tailor-made for a specific development environment. In our case, Jekyll is built with Ruby. Although Cloud 9 has a prebuilt Ruby on Rails template which would work for Jekyll development, we'll select and configure a "custom" workspace.

(Technically, the "custom" workspace type is pretty basic. Later in the book we will examine out to flesh out this basic install and add additional tools to make Jekyll development a bit nicer.)

### Intgrated Development Environment

To begin, it's sufficient to create a workspace using the "custom" template. You can name this as you wish, mine is called "alterego".

After a few moments your new workspace will be created. It comes preinstalled with a version of Ruby which is needed for Jekyll to function properly.

### Installing Jekyll

At this point we can run the "Getting Started" code from the jekyllrb.com website:

$ gem install jekyll

The above command will install Jekyll and its dependencies into your cloud environment. When it is complete we'll have the full power of Jekyll at our disposal.

## The default template

Jekyll contains the ability to generate a new "template" project. This project is a shell for a basic, clean, fully-functional static website.

$ jekyll new my-awesome-site
$ cd my-awesome-site

### jekyll serve

A standard local configuration (on a laptop, for instance) would be configured to serve up your site in a browser witht the default installation. However, with Cloud 9 we do have to perform and additional configuration. (You'll need to remmber this for now, but in the future we will write a few scripts to handle this for you.)

~/my-awesome-site $ jekyll serve --host $IP --port $PORT --baseurl ''

The above command works a little magic to publish your site within your development environment. If all goes well, you should now be able to preview the site in the IDE or in an external browser.

In the Cloud 9 IDE  click the Share button, then click the Application url and choose "open". A new browser window (or tab) should open and display the contents of the base Jekyll theme.

This theme serves as a template and is able to be modified to create a robust static website.

### my first website

The jekyll serve command watches the filesystem for changes. As you change most files in your site it will automatically pick these changes up and reflect them. One exceptin to this rule is the _config.yml file.

This file is a plain-text format file that contorls various options for your Jekyll site.

Let's customize your site to help demystify it a bit.

You'll likely notice a few familiar items in this file. There is a lot of awesome in the default file.

Go ahead and change the title, email, description, twitter_username, and github_username values to relect your information.

You'll need to stop and restart your jekyll server. To do so, hold "control" on your keyboard and press "c". Then press the up-arrow key (a linux shortcut for looking back through the command list) and press enter to reexecute the jekyll serve command.

Switch back to the preview of your site and reload it. It should change to reflect the new values we typed in.

## Version control with Git

### Installation

### Why get Git?

### GitHub

### Branch, edit, commit, merge

## Deployment

### Again, GitHub

## Conclusion

### What we learned in this chapter

## Kata