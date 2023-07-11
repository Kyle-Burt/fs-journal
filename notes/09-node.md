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


<!-- NOTE creating todays project in express-mvc -->
    do not comment out the lines of code from yesterday
    .env should never be pushed up to github
    gitignore is set so you don't push up certain files to github

    monogdb connection - click on DB - drivers - copy connection string paste to connection_string

    database access - to make a password must be HTML safe. click autogen and copy.
    paste in behind username in string 

    auth0 to get remaining info
        -applications, applications, myapp/single page application 
            - get domain, client
            -api tab/ api audience 
        go into client copy info in env folder 

    using ctrl ~ and use run and debug client 

    once you can get connection copy and slack all the info from .env and env.js to yourself so you never have to do it again. Winning like a boss.

    <!-- NOTE schema = schematic -->
    schema let you put validation in the back end too. to help fight off the dink's and buttholes of the web *Dark Web!*

    setup order model, DB, controller, service 

    .use(Auth0Provider.getAuthorizedUserInfo) is middlemare 
    authorization tab, bearer token,
