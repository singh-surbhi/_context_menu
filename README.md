# _context-menu
A very simple, light, flexible and most dynamic context menu on web. Bind your mouse click events ( right click / left click) on any clickable element on your page. (It supports context-menu popup on **DYNAMICALLY created elements**).

**Prerequisite**

1.  Only Jquery

**Syntax**

      $(function(){
                                                 // When document is ready
	    var x = new _contextMenu();              // Create instance of _context_menu
	    x.config({                               // Configure the new context menu
		contextBoxClass : 'context-menu1',
		clickedOnClass : 'class name',
		closeBtnClass : 'className',
		// popupBesideClass : 'className',
		// disableErrorLog: true
	    })
	    x.run();                                 // initiate the newly created context menu
      });


***config* OPTIONs**

 
**contextBoxClass** : 'className',   Class name of the context menu created in HTML

**clickedOnClass** : 'className',    Class name of invoker of the context menu (usually anchor, button, or any mouse click event)

**closeBtnClass** : 'className',     (optional) In case if you have close button to close the context menu, pass the className here. By default context menu closes when clicked anywhere out side the context menu body. 

**popupBesideClass** : 'className',  (optional) Provide the className where you want the context menu to appear when invoked. If not provided by defauly it takes the position of the DOM element responsible for triggering the event ( or mouse click position)

**disableErrorLog** : false | true.  (Optional) By default the value is 'false', which means errors and suggestions will be logged in console. Its handy while setting up the context menu. Make it true if you don't want to log errors in console.
