
## Ardoq test

## Part 1

**"Create a method that, given a list of integers, returns the highest product
between 3 of those numbers. Example: [1, 10, 2, 6, 5, 3] = 300"**


You can view the code at https://jsfiddle.net/andnord/qbf141rp/22/

Logic for solution was that to get the highest product you always want to use the highest numbers in the list.

So simply get the highest number, multiply with sum (starting at 1) and remove it from the list *3

Then return product.



## Part 2

**I went for 2c - "Create a simple chatbot using whichever service or framework you prefer"**

* **The chatbot should include at least 2 commands.**
I interpreted commands as the same thing as Intents in DialogFlow. The two intents this chatbot has is "get bitcoin price" and "meaning of life". (it also has a greeting intent)

* **One of the commands should give a follow-up question.**
The "meaning of life"-intent gives a follow-up question asking for a your name.

* **One of the commands should give an answer from a public API (i.e. Yr,
Coindesk, The Internet Chuck Norris Database, ...)**
The "get bitcoin price"-intent uses the Coindesk API to get the current bitcoin price in USD

* **The chatbot should be able to store an answer the user gives and use it
another question/response**
In the "meaning of life"-follow up, the bot remembers your name and uses it in the next answer.

* **In your submission, include a sample conversation**

part 1:
https://github.com/nordbyandreas/nordbyandreas.github.io/raw/master/img/bot1.PNG

part2:
https://github.com/nordbyandreas/nordbyandreas.github.io/raw/master/img/bot2.PNG 

As you can see the bot doesn't understand anything other than greetings, bitcoin and the meaning of life.

* **In your submission, include a sentence about why you chose a specific
service/framework to solve this task**
I took a quick look at Superscipt, ChatterBot, wit.ai and Dialogflow. They seemed pretty much equal, but some people online preferred Dialogflow and I found some good tutorials to learn from so I chose that.

All of them were new for me, so I didn't have any preferences myself.

Working with dialogflow was good.


* **We should be able to test your submission on our end so include a readme
with setup instructions**

I interpreted this as meaning that you want to test the actual bot. Since the bot is online available for testing I am assuming it is okay that I don't include setup instructions. Just let me know if you want me to include setup instructions anyway !

You can test the bot at www.andreasnordby.com

The webhook used for accessing the Coindesk-API is hosted on Heroku and you can view the code here : https://github.com/nordbyandreas/coindesk-webhook
