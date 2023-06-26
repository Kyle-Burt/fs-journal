# MVC

<!-- SECTION intro to MVC *model view controller*-->

MVC - model view controller 
<!-- *NOTE how to create projects in class now -->
not longer using mkdir to create projects
    bcw create - mvc, 
    don't initialize project can do it through github later

appstate.js - this is where you storage all global variables now 

try not to write out import functions, let tab auto complete write it to avoid problems in code

pop is pre-written code to sweet alerts

place _ before private functions that can't be accessed by the user can't be accessed from the console 
 getter's must return a value, can not take in any parameter's 
 this.whatever 


if you get rid of the main you need to go in and get rid of the router id with the same name set

appstate.js is used to store global info. in-between the {}
of the observableAppState.
<!-- NOTE Controller layout -->
controller is used to create functions, anything you want exported needs to bo within the controller  
    layout - export class CoinsController{
        constructor () {
            console.log()
        }
    }

    replace/add controller to router "don't forget to import to page"

    controller doesn't cause function to work, need to make a service to make working function

    service - create class{}

    export const class = new class 

    private functions have to be declared outside of the export controller, and have to be set as function _drawCoins(), make sure to set id in the html so the function can be injected into the code
        can use setText to inject instead of writing out the whole function.

        if you want to use multiple controllers in the router you need to make the controllers into and array 
        Controller: [controller, controller1]

        listener - AppState.on('coins', _drawCoins)
                    AppState.emit -yells 



<!--SECTION MVC more rules and functions -->
    <!-- NOTE API section -->
    
    API = application programming interface

    when getting objects from API = 
        async getMonsters(name){
        try{
            
        }catch (error) {
            console.error(error)
            pop.error(error.message)
        }

    }
/* NOTE harder way of coding */

    fetch(allows us to make requests from api to receive data)
    async is need to use await = makes JS freeze until the data/json can be rendered/loaded
        if getting promise error might help to add await to code so it pauses to render.

/* NOTE axios script done in index. add above /body tag
    AxiosService.js
        export const zeldaApi = axios.create({
            baseURL: 'make it something generic'
            timeout: 8000, if it takes longer than 8 seconds will throw a message.
        })
                /*NOTE - api.crud method
        const response = zeldaApi.get()

        crud request methods(get, put, post, delete)

        paying attention to scoping. async only has to be made once then await can be used

        /*NOTE - found under network tab
        status: 200 good response - successfully found request
                404 error "Page not found" data requested not found.
                405 error method not allowed

