---
layout: post
title: Best Beaches in Florida CLI GEM!
---

This project was an assignment from the on-line course Learn.co created by the **Flatiron School in New York City**.
The assignment was to build and publish a command line interface (CLI) Ruby Gem that scrapes data from a website and allows the user to interact with the objects created from the scraped data through a CLI.  

####Initial Thoughts.  

There were two parts that were difficult for me. The assignment required a few extra's that the previous assignmnets had not included. These were this blog that you are reading here, and a screen capture of how the CLI  works. Both of these extra's I had never done. So, we were left to our own research to finding out how to complete these. The first place I turned was to 'Ask A Question', which allows your question to be answered by other students and teaching assistants at the school. A very nice student directed me to a website called 
[Build a Blog with Jekyll and Github Pages](https://www.smashingmagazine.com/2014/08/build-blog-jekyll-github-pages/) which proved to be a very easy solution for someone who had never published a blog before. The other 'extra' which i had to learn was how to make a screen capture demonstration of how the program worked. Again, the coummunity at Learn.co had the answer.
Quicktime proved to be very simple, and the demonstration was very easy to produce.  

####Now on to the program.  

The lesson included a video walkthrough of [How to Create a CLI.](https://www.youtube.com/watch?v=_lDExWIhYKI).
It was helpful in getting me started with creating a gem and then writing the code. It offered a sort of error driven approach to writing the code. The demonstrater would write the code frome the perspective of what he wished was available for him to write. He would write code that he wanted to be there and of course this would generate an error because the underlying code had not been written yet. So, he would write the code to correct the error. This is why it is called error driven development. I started off that way, but then swithed to a different approah. i scraped the website for anything that I thought might be interesting to a user and then created the object and menu from there. i dont know if this approach would work for a larger more complex application, but for this contained domain it was fine.  
**A snag along the way** was how was I going to have my three objects communicate with each other. The way I saw it, I had two options. On was to have the CLI ask the Scaper class to pass its data that it scrpaed, pass the data to the Beach class to create  Beach objects and return them back to the Scraper class  which would satisfy the orignal call from the CLI to 'get_beaches()'. I did not do this design. Instead, I chose to have the CLI be the center. It stood between the Scraper class and the Beach class. The CLI asks for scraped data from the Scraper class and the the CLI passes the data to the Beach class.
In this way the CLI acts as the controller, and the Beach and Scraper classses are decoupled. I think this is the better way to go for further changes. 




