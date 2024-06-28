# About pyStructify

## What It Is

pyStructify is a desktop app that handles the boilerplate and creating a project structure for you. With it, you're just a few clicks away from even the most complex project structure being created. pyStructify will also create a virtual environment if desired, create your requirements.txt with the packages you've chosen to include, and optionally install those requirements in your virtual environment. It can also initialize a git repository for the project, as well as create a README.md.

For general projects, you'll create the subdirectories and files that you'll need all within the app, preview your project structure, and then have it created. For Flask projects, you can choose whether or not to use blueprints, and adjust the default boilerplate in files such as `__init__.py` and `base.html`.

pyStructify aims to take the tedium out of starting complex projects, so that you can jump right into the code.

## Inspiration

I've been making web apps with Flask for a few years - or starting them, at least. I always seem to get a shiny new idea before the last one is finished. Because of that, I write the same lines of code *a lot*. Practically nothing changes in `__init__.py` but my blueprint names. The structure for a lot of my projects is the same.

Recently, I tried to learn Django. Gave up on that pretty quickly; Flask is all I need. But something did stick out to me - when you create a Django project it creates a project skeleton for you; some of the folders and files you'll need, boilerplate included. I thought - *Flask needs this*.

Initially this idea lived as a command line flask project skeleton generator on my github, but I wanted something easier. *(Anyone else hate the command line? Just me? Ok.)* So (with no real GUI knowledge), I decided to make a desktop application, and then expanded the scope of it to include general projects as well.

In truth, I set out to automate something minor, but just kept adding functionality. I'm pretty happy with the finished product, and I hope it saves you all some time as well!

## About AprilMay

I'm a self taught hobbyist developer with a love for putting things together. I started learning python in early 2020 and have been obsessed with it ever since. I've started what seems like a million projects, but pyStructify is the first that I really committed to. I really sat down and said I'm not jumping to the next new idea, *I'm going to finish this one*. And after a few weeks, that's exactly what I did! I know it's not some groundbreaking or innovative software, but it's near and dear to my heart and I hope you find it useful.