# Vue

<!-- NOTE new framework simplifies javascript -->

{{}} - used for string interpolation instead of ${}
setup() - private function
return() - public functions 

<!-- NOTE starting structure  -->
src-services setup new axios services
create new axios service if you need to. 

start client and make sure everything is working
homepage.vue is like the main controller page 
remove template code and style code 

set-up key - params: {
    api_key: key value,
}

have to turn a key into a string if .drilling into property

create class model for movie 
store saved data in appstate = movies[]
onmounted() get movies every time the page is activated - similarly to the controller constructors/page load or component load.
double curlies for text content
bind for imgUrls exp. img :src="whatever URL"

refactor into smaller components - 
props goes above setup and return

props: movieProp: {type: movie, required: true}

MovieCard :movieProp="movie"

when to use props or computed. 
most of the time you use props is when you using a v-for *child component*
parent component uses computed. 
computed is a reactive property 

router-link - go in tandem with the routerview.js - text will turn blue within a router link
binding :to="{name: About}"

create a new page.
go back to router.js create new route object

component: loadPage('must be identical to vue page')

ellis operator true false indicator 


<!-- NOTE day4 7-20-23 -->

starting project create function to pull data from setup.
create service.j page to add layer to website 
controller *homepage* -> service
'router-link :to="{name: 'profile', params: {profileId: 'porject.creatorId'}}" params need to match the params stated in router.js, path params 

const route = useRoute()
const profileId = route.params.profileId


<!-- NOTE 7-24-23 -->
express-vue to create project.
postman for this weeks checkpoint
will need two bearer tokens

postman - import - link 
setup postman with all tokens needed 
2 accounts one in normal window, second is incognito window for second account - 2 tokens needed to test against 

must run tests in order of postman tests.

will create data for you. don't change info in the body

create a schema first. models
register schema - dbcontext.js
create controller and service 