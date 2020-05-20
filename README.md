# bulkBotChecker 
![Logo](https://i.ibb.co/25dMcTQ/what-is-bot-traffic-cover-dcfd8e825fc46554db1393c5efb749b1-removebg-preview-1-removebg-preview.png)

Script automating twitter accounts verification process with Botometer API. It automatically enriches data with creation date, a number of friends and followers, verified status, and URL from Twitter bio.

## Installation

`pip install -r requirements.txt`

Don't forget to put API keys into script. 
Script requires standard Twitter API keys and Botometer RapidApi account (https://rapidapi.com/OSoMe/api/botometer-pro)

## Usage:

Check single user:

`python bulkbotchecker.py -u <twitter_handle>`

Check list (csv) generated by Gephi:

`python bulkbotchecker.py -g <filename.csv>`
  
Check list in any text file (one twitter handle per line):

`python bulkbotchecker.py -l <filename>`

### Sample output:

![Output](https://i.ibb.co/c8Ksr1x/output.png)

### Sample summary:

> No timeline accounts: /number of accounts without timeline/  
> Suscpicious accounts: /number of accounts with score above 2 on botometer/  
> Locked accounts: /number of private/locked accounts/  
> Humans: /number of accounts with score below 2 on botometer/  
> Shadiness: /ratio bot/suspicious accounts to human/  
> Network mean score: /score average mean of all accounts/   
> Accounts younger than 30 days: /number/  
> Accounts with less than 10 followers: /number/ 

![Summary](https://i.ibb.co/VLC1k1f/cmd-klm-UIGy6f-K.png)

#### ToDo:
Add functionality to output results to file. 

