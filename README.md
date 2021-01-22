# What are these files?
These are the files of a Python program (a.k.a. App 7) built in the Udemy course  "The Complete Python Course in the Professional OOP Approach."
The course covers how to make this program step by step, plus nine other Python programs. 
If you want to learn Python, you can take the course for a high discount in the link below: 
https://www.udemy.com/course/the-python-pro-course/?referralCode=D1224FDF916B73D7E740
# What does the program do?
The program is written in Python. The app will read the names and email addresses and interests from the people.xlsx Excel file 
and will send an email to each user every morning or at other times of the day. 
The email will contain the news about the user's interest for that day.
# How to run the program
1. Either clone this repo or download all these files by going to _Code -> Download ZIP_.
2. Create a PyCharm (or other IDE) project and configure a Python interpreter for the project.
3. Open the terminal and install the required packages by running:
   `pip install -r requirements.txt`
3. Go to https://www.newsapi.org/, and create a NewsAPI account to get an API key.
4. Go to news.py, and change the string `"INSERT YOUR API KEY HERE"` to your own NewsAPI API key.
5. Create a Gmail account if you don't have one.
   Then go to _main.py_ and change the values of user and password to match your gmail address
   and the password of your gmail account.
6. Go to your Gmail account and set the settings to allow less secure apps
   to send emails from your gmail account.
   Here is a direct link to change the setting: https://myaccount.google.com/lesssecureapps
7. Open the _people.xlsx_ Excel file, delete the current rows (not the header)
   and add at least one row with an email address that you have access to.
   Also, enter an interest in the interest field. The news about that interest
   will be sent to the email address you added in that file.
8. Go to _main.py_, in line 21,and change the hour and the minute values
   to the current hour minute. For example, if your computer shows time
   as 17:22, you can set the hour value to 17, and the minute value to 25.
9. Run main.py with Python.
   Python will hang the execution until your computer time reaches the 
   hour:minute that you set (e.g.,when it is 17:25 is reached).
10. When that timestamp is reached, Python should send an email/-s to the email address/-es
   you entered in the Excel file.