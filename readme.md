![Amnesty International logotype and logo banner](http://amnesty.ca/sites/default/files/ai-lockup-2c-banner.png)

Write for Rights Events
=======================


Every year on December 10th, activists in more than 80 countries gather on their own or in large and small events to press governments to respond to a human rights concern on selected high-priority cases. We also write letters of hope and solidarity directly to prisoners or people experiencing human rights violations. This repo maps and lists community-submitted events.

This project is based on [JLord's](https://github.com/jlord) groovy spreadsheet-based [hack spots](https://github.com/jlord/hack-spots), with the addition of a Google Form as the data source.

## From the original 

### Fork -n- Go!

In a bit I'll do some more refining (and documentation) - but here's a fun fact:

This repo only has a **gh-pages** branch, which means as soon as you **fork** it, you have a hosted and live version of it yourself! 

Next, create a spreadsheet with the same column headers as [the original](https://docs.google.com/spreadsheet/ccc?key=0Ao5u1U6KYND7dFVkcnJRNUtHWUNKamxoRGg4ZzNiT3c#gid=0).

Click on the `index.html` file, click edit and change **line 118** (or thereabouts) it looks like: 

```javascript
    document.addEventListener('DOMContentLoaded', function() {
	  	var gData
	  	var URL = "0Ao5u1U6KYND7dFVkcnJRNUtHWUNKamxoRGg4ZzNiT3c"
			Tabletop.init( { key: URL, callback: showInfo, simpleSheet: true } ) 
    }) 
```

Replace the existing spreadsheet URL key with your spreadsheet's key. You'll find that by clicking (in Google Spreadsheets) File > Publish to the Web > Start Publishing, it will then display the key in a window. ![get key](https://raw.github.com/jllord/sheetsee-cache/master/img/key.png)

Commit those changes and **LIKE WOAH** you now have a version of this website hooked to a spreadsheet that you can distrubute however you'd like.

You can find your version at **yourGitHubName.github.io/theReposName** (in this case /hack-spots).

### But How?

A Google Spreadsheet holds all the data and it is connected to this website using the goodies in [sheetsee.js](http://www.github.com/jlord/sheetsee.js). Everytime you visit the website, you'll have the most up to date data that has been entered into the spreadsheet. 
