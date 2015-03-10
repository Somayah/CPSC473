# Assignment#4


####1.	Briefly describe your team’s project
It is an application for Twitter gateway. We called it as “Twixer.” It will be used by group of users. Each user can login to his account in Twixer and he/she can see all tweets in their account. User can create a group and add other members of the group. User can tweet regarding the group but this tweet will not published on Twitter till the majority of the group members agree with his/her post. Every other member will login to his account will see the groups which he/she assigned to. The member can access the group and see what posts have not been published yet and vote for it. Each voting will be shown as a green sign, while every reject will be shown as red sign. The non-voting will be shown as grey. User can edit, delete his/her posts only if it is not published.

#### 2.	&  3. List of APIs and functionality 


#####Twitter REST APIs
*	Get a Tweet
	
 https://api.twitter.com/1.1/statuses/show.json?id=210462857140252672

 It returns a tweet which specified by the id parameter. The user who post this tweets will also be shown within the tweet.
This API can be used in Twixer application to call specific tweet that has been created but not published yet in order to vote.
*	Get a user search

 https://api.twitter.com/1.1/users/search.json?q=Somayah_Baflah&page=1&count=3

 It returns a list of user as a result of user search. Its parameters are the q=name of the user, page= number of the results’ pages, and count = the number of potential user results to retrieve per page.
This API can be used in Twixer application to search about specific user that can be added as group member.
#####Twicher API
*	Get a user's information

 http://twitcher.steer.me/user/[username]?key=aqneegnh
  
  It returns information about specific user which specified by the username. It pull the Twitter data without asking for OAuth key.
This API can be used in Twixer to show all the user information once the user login in his/her Twixer account.

#### 5.	Describe why you chose that particular API and provide a link to its documentation
I use the Twicher API to get user’s information because it works without authorization key. Also, other group members or users need to know more about the user who add them in group, so they can see their information in Twixer easily instead to login in Twitter.com and check their information.

The link: http://twitcher.steer.me/

#### 6.	Discuss any potential issues that you can foresee with using this API in your project
The potential issues that can be occured are :
*If the user enter wrong user name the API will show the message that “You have entered wrong number”
*If the user click on search for the user and he did not enter the user nam, this message will be shown "Please enter Twitter username"

#### 7.	Evaluate your experience creating the example web page and make a recommendation of whether your team should use this API or keep looking for better options
I would recommend using this APT because from creating the web page I have add input field the request the username just as the login page. Thus, once the user login in Twixer the user information should shows. Also, when the user search about a user to add in a group, the user will enter the member’s username in input field and see the member’s information as I have done in my example. Then, there will be button to add or search again.
  	


