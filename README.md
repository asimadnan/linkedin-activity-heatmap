# Linkedin Activity Heatmap

This repo will guide you how you can create activity heatmap of your linkedin profile.

![alt text](images/asim-heatmap.png "Asim's Activty Heatmap")
![alt text](images/meri-heatmap.png "Asim's Activty Heatmap")

## The Data
To create this heatmap we require post data of the user. it would be quite easy if there was a native API available by linkedin which we could use to fetch posts of any user. 

So what do we do??

we can scrape, but from what i have read online seems like its risky to scrape linkedin, firstly its prohibited by them, secondly i have heard them banning account that they detect were scrapping.

I have seen some paid APIs available that provide scraping servics, and from what i understand they probably use dummy account to run scraping and keep creating new ones if they get banned.

So scrapping is out of question so how do we get all of the post data??

I found an intresting way to fetch this data, using Kleo. If you have not used Kleo its a very useful extension, that shows you top post of any linkedin profile, it mainly works for famous creators, but you can see all posts of any profile, sort them by likes, comments etc.

they show these posts in sidebar on top on linkedin page, when i saw that i thought, they must be storing this data on there server.

I inspected the network calls that kleo makes and voila found something

so long story short i bypass kleo's call to its server to fetch the data.

then save it as json and create my heatmap.

