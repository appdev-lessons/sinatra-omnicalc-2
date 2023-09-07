# Sinatra: Omnicalc 2 (debugging)

In this project, we'll practice forms by debugging and building out some starter code.

Here is our target: [omnicalc-2.matchthetarget.com](https://omnicalc-2.matchthetarget.com/)

Load the assignment and set up a codespace:

LTI{Load Sinatra Omnicalc-2 assignment}(https://grades.firstdraft.com/launch)[S9ymPy6WCsn18gLbByVbZQ7k]{vfdtzJb5bLYqYwuqgeRKpc5d}(10)[Sinatra Omnicalc-2 Project]

Launch your server with `bin/dev` and when you are ready to get automated feedback run `rake grade`. Before you run `rake grade` you should try and manually match the target; don't rely on `rake grade` entirely to debug.

## Objectives

Explore [the target](https://omnicalc-2.matchthetarget.com/) and get your live app preview to match it. There is already some starter code in the `app.rb` file and in the `views/` folder, but there are some bugs in it and there is still a lot of missing code. 

Use the code that is already there along with what you learned about forms in the _Sinatra Omnicalc 1_ project to make progress and get all of the `rake grade` tests to pass.

## Better Errors: Navigating the backtrace frames

Recall [when you learned about the `better_errors` gem](https://learn.firstdraft.com/lessons/103-our-first-sinatra-app#better-error-pages) that we are including in all of our projects. On the right we expect to see a snippet of _our_ code where the error is arising. However, because of the way some errors propagate through the different files (including the hidden files located _inside_ of the gems we are using), sometimes the first snippet of code that you see and the REPL associated with it will _not_ be from your code!

That may confuse you, but here's what you need to do if you see code that you don't recognize (keep an eye on the file path at the top of the code, it should point to one of the files in your Codespace):

On the left side of the `better_errors` window you will see a pane with the "Frames". Click through these frames until you find _your code_ on the right side pane. It will usually be near the top in the second or third frame.

Here's an example of this in action for this project, where you should be relying heavily on the `better_errors` page to help you diagnose issues with the code!

<!-- ![](/assets/better-errors-frames-click-through.gif) -->
![](https://res.cloudinary.com/dmxgp9oq2/image/upload/v1689290665/better-errors-frames-click-through_khlvbi.gif)
{: .bleed-full }

---

- Approximately how long (in minutes) did this lesson take you to complete?
{: .free_text_number #time_taken title="Time taken" points="1" answer="any" }
