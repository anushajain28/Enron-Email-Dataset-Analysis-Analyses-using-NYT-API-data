# Question 1 - Analyzing the data of Enron scandal

## Introduction

Enron Corp. is a company that reached dramatic heights, only to face a dizzying collapse. The story ends with the bankruptcy of one of America's largest corporations. Enron's collapse affected the lives of thousands of employees and shook Wall Street to its core. At Enron's peak, its shares were worth $90.75, but after the company declared bankruptcy on December 2, 2001, they plummeted to $0.67 by January 2002. To this day, many wonder how such a powerful business disintegrated almost overnight and how it managed to fool the regulators with fake, off-the-books corporations for so long.

## Data Source 
[Enron Data](https://www.cs.cmu.edu/~./enron/enron_mail_20150507.tgz "Enron Data Link")

## Analysis 1
As it was a huge scam, tracking the activity of each employee is important. Investigating the sent-mail folder of each employee gives us an idea of what information that person was communicating through his mails. Identifying the trend of mails sent each year and each month during that year might suggest the duration that was critical during this scam.

### Analysis 1 : Identifying the trend of number of mails sent during each year and month

### Steps followed: 
    
- read all the relevant files from sent_mail folders of each employee
- extract year and month for each mail
- calculate the count of mails for each year and month
    
### Results:
 
#####Emails  sent in 1990   
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%201/Analysis%201/Emails_SentIn_1999.png)
#####Emails  sent in 2000
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%201/Analysis%201/Emails_SentIn_2000.png)
#####Emails  sent in 2001 
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%201/Analysis%201/Emails_SentIn_2001.png)
#####Emails  sent in 2002
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%201/Analysis%201/Emails_SentIn_2002.png)
    
### Conclusion:
    
From the results it was evident that there was a sudden increase in the number of mails sent during the end of 2000 and begining of 2001. This was the time when the scam happened. 

## Analysis 2
As it was known that the scam occured during 2000-2001 , and from the results of Analysis 1 it became more evident that something suspicious was happening in the company during that time, so mails sent during that period were analysed.

###Analysis 2 - Determining who sent the most mails and to whom. 
    
### Steps followed: 
    
- read all the mails for the duration 2000 and 2001
- extract 'to' and 'from' from the email data 
- In case of multiple email addresses in 'to' tag, separate each address and store it individually. 
- count up the total number of mails sent by each employee and the count of mails sent to every other employee
    
    
### Results:

##### Who sent the most emails
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%201/Analysis%202/MailsSent.PNG)

##### To whom the mails were sent
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%201/Analysis%202/From_to.PNG)

#### Conclusion: 
Few of the people who were aware of the scam or were involved in it were Vincent Kaminski, John Arnold and Drew Fossum. As we can see from the results, that these people were among the top 10 people who were sending mails during that time.

## Analysis 3
Results of Analysis 2 gave us an idea of who might the key players involed in the scam. Studying the content of the mails forwarded by these people will give an impression of what were the topics of discussion during that timeframe.  

###Analysis 3 - Determining the frequecy of words used during communication via email. 
    
### Steps followed: 
    
- scan the mails of the top 10 people in the list who have sent the most mails.
- extract the subject from the mails 
- determine the frequecy of most common words used and plot it as WORD CLOUD.
        
### Results:

##### Word Cloud of most common terms used in emails of few of the key persons
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%201/Analysis%203/CommonTopics.png)

### Conclusion: 
From the Word Cloud we can see what was being talked in these emails mostly. Looking at the result , these emails were mostly about Deal, Agreement, Meeting, Project. These topics might be used to discuss the scandal that was going inside the company.

======

# Question 2 - Perform the analysis on NYT API data.

## Introduction

NYT developr docs has articles from various categories like books, movies, article search and archives.

## Data Source 
[NYT Data](http://developer.nytimes.com/ "NYT Developer docs")
Download the data and store as json response.

## Analysis 1 
Analysis 1 is based on Article Search API . It has Times articles from 1851 to today, retrieving headlines, abtracts and links to associated media for various domains like Sports, Business, Politics, World etc.

### Analysis 1 : Identifying the trending sports during a particular timeframe.
(Data used for years 2015-2017)

### Steps followed: 
    
- read all the files from Article Search API which have section name : Sports
- get the sport name from the subsection tag of the json data of the file.
- calculate the count of articles published for a particular sport in a particular monthof an year.
    
### Results:

#####Trending Sports During 2015    
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%201/Sport1.PNG)
#####Trending Sports During 2016
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%201/Sport2.PNG)
#####Trending Sports During 2017
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%201/Sport3.PNG)
    
### Conclusion:
    
Based on the data available, the results show the most trending sport during each month of the year.

## Analysis 2
Analysis 1 is based on Archive API . It has Times articles from 1851 to today, retrieving headlines, abtracts and links to associated media for various domains like Sports, Business, Politics, World etc.

###Analysis 2 - Identifying the topics discussed about Mr. Donald Trump. 
(Data used for year 2014, 2015 and 2016)  
### Steps followed: 
    
- read all the files from Archive API for the year 2014,2015 and 2016 which have Donald Trump in the headings of the article. 
- get the abstract of the article.
- compute the frequency of words related to Trump in the articles and plot the WORD CLOUD.
    
    
### Results:

##### Most Frequent Words realated to Trump in 2014
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%202/2014_Trump.PNG)

##### Most Frequent Words realated to Trump in 2015
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%202/2015_Trump.PNG)

##### Most Frequent Words realated to Trump in 2016
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%202/2016_Trump.PNG)

#### Conclusion: 
The results show how the trend of topics related to trump has changes over period of years. From the Word Cloud for year 2014 is can to interpreted that there were not much discussions about Mr. Trump in the news. As the election time approached, in 2015 the discussions about him increased and terms like presidential, campaign, Republican became frequent. And as we had elections in 2016, Donald Trump was discussed the most in the new articles and the frequency of election and Republican party related words became more frequent in the news.
 

## Analysis 3
Analysis 3 is based on Most Popular API . It has Times articles with their view count and shared count and the atricles which were forwaded as email.

###Analysis 3 - Determining the most popular author based on the view count and the share count of his/her articles.
    
### Steps followed: 
    
- read all the files from Most Popular API.
- get the count of total share and count of views of the article.
- get the author of the article 
- compute the total shares and total views for each author
- based to highest total shares/total views determine the most popular author.
        
### Results:

##### Share and View Count of Articles for each Author
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%203/Share_View%20Count.PNG)

##### Most Popular Author
![alt tag](https://github.com/anushajain28/Midterm_Spring2017/blob/master/midterm/Question%202/Analysis%203/MostPopular.PNG)

### Conclusion: 
From the result it can be inferred that these are the authors whose articles are shared and viewed the most.  
    
    



