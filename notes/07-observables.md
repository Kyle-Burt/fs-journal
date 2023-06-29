# Observables

/*NOTE - API's area thing now will be pulling data from them for the remained of the course. we will be building them at some point.

/*NOTE - will be using mvc auth - for todays project works the same as mvc - will have an auth to do before getting started. will have to remove auth code and all scripts have been rendered in code all ready.
NEW env file - Environment* once setup just copy and paste. change baseurl in env.


/*NOTE  CRUD - Create/post, read/get, update/put, delete/delete*   / cat in cdm will open file in cdm

/*SECTION - creation make a controller test it add nav to bar to get to new page controller.
create service file and object.js - copy and paste as dataWhatever = use to choose which properties your object will have.

when pulling from an API async, wait / try-catch.

static get - 


/*NOTE - first things to do - 
    change in env.js to similar links from bcw sandbox
        -domain url
        -audience 
        -client Id
        -baseUrl
    
    make request to api to get info from serve/create another axios if needed 
        export const dndApi = axios.create({
            baseURL: 'URL',
            timeout: 8000
        })

    make a controller, 
    export class SpellsController{
        constructor(){
            console.log("working)
            this.getspells()
        }

        async getSpells(
            try{

            } catch{
                console.error(error)
                pop.error(error.message)
            }
        )
    }

    check if controller is working after replacing values in router and updating index.


    make service 
        class SpellsService {
    const res = await dndnApi.get('api/spells')
    console.log('got spells', res.data)
        }
        export spellsService = new SpellsService()

        set appstate class

        create a draw function in controller.

    






