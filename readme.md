# Twitter Emoji Map

+ **Intro**
	- This is a nodejs project using express as framework and mongodb as data storage. As any other express project, it contains a server and a client.
	- Server observes the newest twitts people sending over the world and seperate them into different groups based on the geo location, in other words, their countries. Note that, it only collects twitts with emojis as the name suggests. After forming groups, it performs a simple statistics on the emotion. It counts the ratio of twitts with negative emojis against positive emojis. And show it on a map that is based on [**a third party public project**](http://echarts.baidu.com/).
	- And using the client on local browser, you can choose to see different ratios during some time interval that goes from 24 hours ago till the current time.
+ **How to run under windows**
 	1.  Pre-install: [**mongodb community edition**](https://docs.mongodb.com/manual/administration/install-community/) + [**Nodejs**](https://nodejs.org/en/)
	2.  Clone/fork/download this project from [**github**](https://github.com/Inverse1Luo/twitter-emoji-map.git) to your local storage. And we say the path of local storage is 'path_to_project'.
	3.  Open terminal -> cd path_to_project -> npm install ->  mongod --dbpath E:\twitter-emoji-map-new\data\db -> npm start
+ **How to use**<br>
Make sure you have internet access to twitter first, because data is retrived from twitter. Open a browser and go to '127.0.0.1:3000'. Once a world map is present, you can select a time interval by a slider on the bottom left and click confirm button to start counting twitts.
+ **Others**
	- All the old data inside mongodb will be cleared once the program starts. Don't worry about your storage space.
	- Give some time for the server to collect twitts before you see meaningful statistics.
---
