## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
  * A cookie is a way to store information between sessions, as HTTP is stateless
* What’s the difference between a session and a cookie?
  * Session is essentially an encrypted cookie
* What’s a flash and when do you want to use flashes?
  * A flash is sorta like a cookie, and it is used to pass messages between requesets
* Why do people say “HTTP is stateless”?
  * There is nothing remembered from the previous state (other than cookies, session, and flashes)
* What’s authentication? Explain.
  * Authentication is how the website knows you are who you say you are. This is typically done with username/password
* What’s the difference between authentication and authorization?
  * Authorization is what a user is allowed to do (after the user's identity has been authenticated)
* What’s a before filter?
  * It specifies a method that will run before any controller actions are run
* How do we keep track of a user once they’ve logged in?
* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
* At a high level, what tools can you use to implement authorization? How would you use them?
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
* What are some strategies you can use to keep your views DRY?
