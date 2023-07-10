<!-- NOTE node lecture/BCW create node-server-auth0-->

-writing our own API this week
still using MVC pattern

<!-- NOTE comment out these lines of code -->
comment out DbConnection.connect() - in main.js
comment out Auth0Provider.configure({}) - in Startup.js

<!-- NOTE starting -->

click run and debug/green arrow start server
localhost 3000
server - controller - standard start.
inherit = extend "BaseController"
super(api/object name"cats, dogs, DBZ, ect.") calls Constructor from baseController
add router/ this.router 
    .get('', this.getcats) - all comes after the router

    every method written in the controller needs to have 3 arguments (req, res, next)
<!-- NOTE order matters always req, res, next -->
    req = request, info need from client 
    res = response, gives info back to user 
    next = error handling *try/catch*

    restful convention = api/cats/id - id is the RC that comes after cats

<!-- NOTE must re-spin the server when checking changes/console.log not used -->
new tool postman api platform - get used to working with it because it will be a vital part of the testing process for future projects.



