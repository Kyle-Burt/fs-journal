# MVC

<!-- SECTION intro-->

MVC - model view controller 

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