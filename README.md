# Final Fantasy XIV Stone Sky Sea Calculator

The Stone Sky Sea Calculator is a tool for the MMORPG (Massively Multiplayer Online Roleplaying Game) [Final Fantasy 14](https://eu.finalfantasyxiv.com/). 

Online gamers can be very competitive and want to compare themselves to other players. While the game provides a way to measure your strength by fighting a training target, it is a binary result - You either beat it or you don't. This is where this tool comes in. By taking the only pieces of information this training target provides, the health and time, a player can turn their binary result into a number that can be compared to other players.

## Future changes

I started this project when the number of available fights was pretty small (less than 5) but over the last two years this number ballooned out of control. Right now there are 36 different fights with 15 classes each, so 540 data points in total. My initial data structure is still working fine but it gets harder and harder to keep the data updated.

I want to do the following changes to my data structure

* Group similar fights
* Group fights by game expansion
* Store HP data inside fights instead of inside classes

These changes should make it easy to then use a templating engine like Handlebars or a larger framework like Angular to generate the HTML from my data. This would separate the model from the view and make it so I only need to edit the data to add a new fight (instead of editing the HTML as well right now). 

I also want to update the design of the website to make it cleaner looking and a bit easier to use and also provide translation options into German, French and maybe Korean.