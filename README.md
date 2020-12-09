# FifaIndex
A scrapy web crawler to scrape player's states from www.fifaindex.com

# Requirements
* python 3
* Scrapy 2.4
```
pip3 install -r requirements.txt
```

# Fields
A player item has 60 attributs
* Player's overall and potential, height and weight (cm, Kg)
* Player's preferred positions, weak foot and skill moves (out of 5 stars)
* Player's preferred foot (R/L)
* Player's birthdate and age
* Player's value and wage (€)
* Player's Nation (position and kit number) and Club (position, kit number, date joined and contract length)
* Ball skills (ball control, dribbling)
* Defence (marking, slide tackle and stand tackle)
* Mental (agression, reactions, att. position, interceptions, vision and composure)
* Passing (crossing, short pass and long pass)
* Physical (acceleration, stamina, strength, balance, sprint speed, agility and jumping)
* Shooting (heading, shot power, finishing, long shot, curve, FK acc., penalties and volleys)
* Goalkeeper (GK positioning, GK diving, GK kicking and GK reflexes)
* Player's Specialities
* Player's traites

# Scrape player's stats
### From the current year
```
cd FifaIndex
scrapy crawl players
```
### From a specific year 
```
cd FifaIndex
scrapy crawl players -a link="https://www.fifaindex.com/players/fifa16/" 
```
### Save stats to a file
```
cd FifaIndex
scrapy crawl players -o out.csv
```

# Dataset
The players spider used to generate the following dataset
* [Fifa Players](https://www.kaggle.com/justdhia/fifa-players)

License
----

MIT

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
