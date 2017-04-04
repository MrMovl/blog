Title: Better Elm
Category: programming
Lang: en
Date: 2017-04-03
Tags: elm programming 
Status: draft

# Could we solve the component problem with this little trick?

Excuse the BuzzFeedesque title. I felt witty and noone stopped me.

### What is the most controversial topic in the elm community right now?
I have the feeling it's components. And to be honest, i don't really understand why this drives people so mad, but I do accept the longing for a componenty solution as well as the reservations from the more functional thinking of the core team. And I tend to agree with the solution of rather compartmentalising your functions in this beautiful functional language, than insisting on building small building blocks with their own small _The Elm Architecture_ (henceforth TEA). Then again, I don't believe I am experienced enough to dismiss the people convinced that there is a need for components.
But, why not think about a solution instead of getting into the trenches and shooting at each other with hurtful word-bullets?

### Let's characterize the problem real quick

So, turns out programmers are lazy. That is generally what drives us to come to clever solutions for repetitive tasks. So naturally, if we build, let's say, a credit card input form, we want to use it in more then one project. So we wrap it in some sort of container so we can just drop it in several places and use it there. This container is called differently in other languages, but in elm this would be a module. As an interface for this module we have imported functions from other modules and exported functions for other modules to use. But in order for TEA to help us with the pesky interactions with the outside world we need to shove all of our user interactions to one designated module containing our main model, main view function and main update function.

*This is not really true... I need an example to clarify, maybe something with a main module and a sub module. The main module has a counter ticking the seconds and the submodule had a button to reverse the direction*