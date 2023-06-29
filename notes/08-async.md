# Async


used for some api's under the baseURL and timeout
params {api-key: 'object key'}


<!-- NOTE  order of build -->
    update evn.
    don't add /api to base url
    check network to make sure you're getting the proper codes 
    build secondary API's for any other api that will be in use 
    paste in browser to make sure it works and a request can be made
    make a controller,
        -separate APIS one for each api used so they can talk to one another separately 
    /* NOTE build application structure in index and then copy/paste to appropriate spot later in code
        -remove text and update router and index 
        -make request to api 
        async/await, try/catch, errorlog 
    setup service 
        make method to service from controller to get api 
        always starts with const res=
        once method created make sure to call function in controller
        copy object and make a data model 
        shave properties down to what you need to save to sandbox api
        slug is used as a special id usually 
        can use bracket notation to drill into specific files ['']
        set pic in appstate
        set draw function 
        to change body background
        let htmlbody = document.body
        htmlBody.style.backgroundImage = `url(${picture.imgUrl})`
        can set background images through css 
        search bar = div/form/input/button
        form onsubmit = app.apicontroller.getRandomPicturebyQuery()
        create template 
        setHTML()

        set event.preventdefault()
        let form = event.form
        let formdata = getFormData(form)  <-must be imported 
        /*NOTE - don't forget to put a name on the input field 
        
