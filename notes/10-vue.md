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
