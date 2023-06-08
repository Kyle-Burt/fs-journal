# Bootstrap

giant css library 
make website developing easier
links similarly to MDI cdn
    bootstrap container *contains rows within the container*
        multiple rows within container *similar to flex box*
        upto 12 columns within a row *can make 4 flex boxes by combine 3 columns* 
        `<div class=container>
            div class=row
                div class=col
    basic layout container-row-col
    container will have margin container fluid does not 
    dev tool can be used in tandem with bootstrap
        bootstrap has tons of utilities *check bootstrap utilities on webpage under docs*
            avoid putting margin on column in bootstrap on x axis
            padding on x axis is more recommended 
            sticky-top will stick to body or parent 
                *margin=m or padding=p you can add e,s,x,y to set specific*
                colors *text, background, ext.*
                fs-2 stands for font size 2, font=f can have any css font properties*
                align is for y axis?
                imgs are read as text so you can use text alignment ie*text-center* 
                img-fluid keeps img within the bounds of the colum does not resize to larger size 
                when setting limitation do base col12 md-6 lg-4
                    *base, medium break point, large break point*
                        also works for padding
            a-tags are used for hyper links adding a target _blank will open in new tab
                 

        .whatever will add class to a div

        @media will allow changes to be made based on screen size *place media rules at the bottom so they are read last in the page and will be applied 

        ex. @media (limiter *max width: 768px will){*css rule* change from orig to new rule set}
        media rules written work in tandem with BS media rules just match px count for sizing.
        set parent to position-relative when set column to position-absolutely so that the item is being snapped to it will stay with the relative 