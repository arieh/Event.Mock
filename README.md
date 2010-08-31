$count
========
This little wrapper creates a Mock Event object to be used with fire event.


How to use
----------

The simplest use case is this:

    #JS
    $('el').fireEvent('click',new Event.Mock);
    

If you want, you can set a target for the event:

    #JS
    var ev = new Event.Mock($('el-target'));
    $('el').fireEvent('click',ev);
    
    
And lastly, you can specify an event type, though this will not be used on IE:

    #JS
    var ev = new Event.Mock($('el-target'),'mousedown');
    $('el').fireEvent('click',ev);
