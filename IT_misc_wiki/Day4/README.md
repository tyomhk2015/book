<a href="https://github.com/tyomhk2015/book/tree/main/IT_misc_wiki" rel="noopener noreferrer"><b><< Back</b></a>

# Day 4

From chapter 16 to 21.



### Chapter 16

<b><i>Extinction of Internet Explorer</i></b>

Didn't know until I read the book that `IE` was popular back in the days, the first browser that adopted CSS and Ajax. Often used it for surfing the internet to find games.

According to the book, the reason of the IE's extinction is due to the laziness, and believing too much on the share that IE possessed in the past.

Cannot provide any evidence, but I believe there might be some political issues within the IE team. It can be an issue related with compensations, the borders were neglecting the reality and potential threats to IE.

Takeaway, or a lesson, from this chapter was that the `one being in comfort zone will be deteriorated`, and I feel this does not only apply to IE but also in real life.


### Chapter 17

<b><i>Cookie, in web development context</i></b>

Web browsers, in most of the time, communicates via HTTP. However, once a request is done, the server terminates the communication because its job is done, and does not keep track of the state of users, aka `stateless`.

To solve this problem, cookie was invented. Cookie is like a ticket or reciept that clarifies who the user is, and shows preference of the user for using a specific web service.

When a browser sends a request to server, cookie is sent together. By checking the cookie, server can know who the user is can show contents that are exclusively for cerified user of a specific web service.

```
  Rules of cookies.

  1. One cookie is for one domain.
  2. Cookie will be send with a request automatically.
  3. Cookies are stored somewhere in user's hardware.
```

If some blog post possesses a Facebook's `like` button link, the Facebook can obtain some information related to any that is in the blog post, because a request is being sent from a blog post from different domain by user's interaction.

On the top of my head, there were a new rule related to cookies being exploited, and this was a huge issue to many advertising firms that were relying heavily on cookies for their marketing purpose.


### Chapter 18

<b><i>The term of `Frontend` and `Backend`</i></b>


Frontend, developing the part where user visually interacts. For example, a browser.

Backend, developing all the logics and data that are essential for running a software.


### Chapter 19

<b><i>The meaning of `server`</i></b>

Literally, a server is an entity that waits your order and does something for you. A server in a restaurant and a server in web development is alike.

Server is like internal organs for web developmet, which must be active all the time. In case of the server becomes inoperable, some disater recovery plans are must be set beforehand.

In South Korea, there was an infamous server disaster cause in autumn of 2022, which made the number one messenger inactive for more than six hours. Not only the chatting, but also other related services that depended on Kakao were unavailable.

This gave a lesson to many people who resides in South Korea that depending on only one method or meaning is risky, alternative plans are must be prepared, like using LINE instead.



### Chapter 20

<i>The term `Full stack`</i>

To put it simple, Full stack = Frontend + Backend + Devops.

There are some companies willing to hire a full stack developer, because they believe the one full stack developer can perform that could be done by two or more people. This is a red sign, a sign that they are trying to exploit the developer. Some do expect that a full stack developer knows EVERYTHING related to web developement, which is hardly true.

To prevent from such companies, ask how many members are in the team you are going to be participating, and clarify the range and responsibilities related to the job and tasks.


### Chapter 21

<i>The term `Serverless`</i>

Serverless sounds like there is no server, but the real meaning is that the developer do not need to configurate server manually, like on-premise. Buying expensive server machine and parts for the machine is no longer needed. Those configurations are done and maintained by serverless providers.

Amazon provides EC2, a virtual machine in cloud for running a server, which was a new solution for problems when using on-premise. The problem with the IaaS, Infrastructure as a Service, was the the developers had to configure OS of the machine, security and disaster issues manually. Due to this inconvenience, `serverless` was introduced.

`Serverless` to take care of most of the problems that were mentioned above. All the logic are uploaded to `serverless` cloud, and the server is put into sleep mode if no logics are called. Any logics are to be called, then the server will wake up and take care of the incoming requests. This is very efficient for in context of energy and money.

Personally, I have used Google cloud function, which is a serverless, before and the first thing I noticed was the very first request was taking longer than I was expecting. The time required for a computer to awake up is called `Cold start`, this is done by calling any functions that are in the `serverless` cloud.

Another cons of `serverless` is that the developer and business logic is coupled tightly to one provider, CGP or AWS. In order to migrate from one enviroment to another will cost a lot of time.

The `serverless` is for...
```
  1. The ones that are making MVP, minimum viable product.
  2. The ones to save time of configuration and focus more on product.
```

<hr>

 #노마드코더 #북클럽 #노개북