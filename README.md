# FallHacks23
Cole, Hannah, Jake, Christian and Andy's Fall Hacks submission








# Leaderboard Stuff - A Dynamic Static Site

## https://jakeyee.com/leafderboard




The leaderboard of the site is hosted as a Static site on Cloudflare Pages. This introduced a number of technical problems, each of which had a technical solution, with in turn introduced another technical problem. This continued until the snake started eating its own tail and the technical problems started becoming technical solutions. 

The flow of the backend is as follows:

![path](https://github.com/Masagoro1/FallHacks23/assets/99901262/a1f98001-6e95-4d4b-bfb9-8cb4fb8b9058)

User Wins game and uploads score  


This score is sent to Discord via a Webhook  


From here, a Discord Bot receives this message  


A python script on my computer receives this message from the bot  


Saves the scores to my computer  


And creates a javascript file containing all the scores  


This file is uploaded to a github repo via the Github API  


Before being sent to GitHack, to cache the file and make it available  


A seperate static site hosted on Cloudflare Pages requests the file  


Which generates an html table and and it visible to the user.  
