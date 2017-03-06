# Question 1 - Analyzing the data of Enron scandal

## Introduction

Enron Corp. is a company that reached dramatic heights, only to face a dizzying collapse. The story ends with the bankruptcy of one of America's largest corporations. Enron's collapse affected the lives of thousands of employees and shook Wall Street to its core. At Enron's peak, its shares were worth $90.75, but after the company declared bankruptcy on December 2, 2001, they plummeted to $0.67 by January 2002. To this day, many wonder how such a powerful business disintegrated almost overnight and how it managed to fool the regulators with fake, off-the-books corporations for so long.

## Data Source 
[Enron Data](https://www.cs.cmu.edu/~./enron/enron_mail_20150507.tgz "Enron Data Link")

## Analysis 1
As it was a huge scam, tracking the activity of each employee is important. Investigating the sent-mail folder of each employee gives us an idea of what information that person was communicating through his mails. Identifying the trend of mails sent each year and each month during that year might suggest the duration that was critical during this scam.

### Analysis 1 : Identifying the trend of number of mails sent during each year and month

### Steps followed: 
    
Markup : * read all the relevant files from sent_mail folders of each employee
		 * extract year and month for each mail
		 * calculate the count of mails for each year and month
    
### Results: 
    
![alt tag](https://www.w3schools.com/css/trolltunga.jpg)
    ![alt tag](image_url)
    ![alt tag](image_url)
    ![alt tag](image_url)
    
### Conclusion:
    
From the results it was evident that there was a sudden increase in the number of mails sent during the end of 2000 and begining of         2001. This was the time when the scam happened. 

## Analysis 2
As it was known that the scam occured during 2000-2001 , and from the results of Analysis 1 it became more evident that something suspicious was happening in the company during that time, so mails sent during that period were analysed.

###Analysis 2 - Determining who sent the most mails and to whom. 
    
### Steps followed: 
    
..* read all the mails for the duration 2000 and 2001
..* extract who sent the mail and to whom 
..* count up the total number of mails sent by each employee and the count of mails sent to every other employee
    
    
### Results:
        
        
    
    



