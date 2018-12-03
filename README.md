Survey link: https://docs.google.com/forms/d/e/1FAIpQLSeJKSjN6gjzJ4XLaTtddQBHMCDKGucuG9zFsV63TPwA1w4MQA/viewform

Code referenced for pulling data from Google Form to local 
http://pbpython.com/pandas-google-forms-part1.html 


# IEOR 4501 Project：Restaurant Recommendation Tool for Group
### Section: 002
### Group Members: Di Wang(dw2839), Jia Yin Yu(jy2945), Shenghui Hua(sh3590)
<br>

## Main Objective
Deciding where to eat can be difficult for a group. Although there are plenty of restaurants nearby and many apps that recommend where to eat, rarely anything exists for optimizing the group decision. Everyone has their own preferences and it’s hard to come to a final conclusion. To solve such dilemma, our group plan to create a recommendation system for group decision making. We would like to take everyone’s preferences as inputs and generate the most optimal solutions based on the current options available. <br> 
<br>

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Python 2.7 or later
Google developer's account (for API key)
Microsoft Word



### Installing

Our first block of pip install was for connecting Google Forms to the Notebook  
```
!pip install gspread
!pip install oauth2client
!pip install oauth2client --upgrade
!pip install pyopenssl
!pip install pyopenssl --upgrade
!pip install pyasn1
!pip install httplib2
!pip install payasn1-modules
!pip install rsa
!pip install six.py
!pip install pycrypto
!pip install httplib2
!pip install ssl
!pip install --upgrade google-api-python-client
```

In order to scrape date from Yelp, we installed BeautifulSoup
```
!pip install bs4 
```

As part of our algorithm, we require numpys and pandas for the calculation.
```
!pip install pandas
!pip install numpy
!pip install re
```

Twilio is the library for sending text message to users
```
!pip install twilio
```

The following libraries are used for generating word cloud
```
!pip install wordcloud
!pip install matplotlib
```

The following library was used for generating the map

```
!pip install folium
```

The following library was used for generating the word document

```
!pip install python-docx 
```


## The process

First, we send the survey link to group users for their individual preferences. Each member of the group submit 1 response. Then, our program analyze the individual preferences and generate a recommendation based our algorithm. The result will be returned to users' phone via text or email(word document) after run our super awsome algorithm. The document contains summarized information about recommended restaurants, including phone numbers, address and some recommended menu items. Alternatively, if the user prefer other restaurants, we have provided two other choices. 



## Deployment
You will need to set up a goolge form like this:  https://docs.google.com/forms/d/e/1FAIpQLSeJKSjN6gjzJ4XLaTtddQBHMCDKGucuG9zFsV63TPwA1w4MQA/viewform
Connecting to Google form requires secrete JSON key from google account  
In order to keep privacy, we have not listed this information on GitHub. A member from the group will email the instructor the file used in the code, "Restaurant-key.JSON"
If you want to activate SMS Text to phone by python, please email me for API code.
Since we are using Twilio account's free trial account (college students are poor), it has some limitation, eg. users' phone# need to be verified before we can send text to them. However, if you upgrade it to full account, their will be no restrictions. Also the address on the text is clickable (linked to your map app).
Add additional notes about how to deploy this on a live system


## Acknowledgments

* Emotional dictionary: https://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm
* Send text message: https://www.twilio.com/docs/api
* Write doc: https://python-docx.readthedocs.io/en/latest/
* Survey link: https://docs.google.com/forms/d/e/1FAIpQLSeJKSjN6gjzJ4XLaTtddQBHMCDKGucuG9zFsV63TPwA1w4MQA/viewform

