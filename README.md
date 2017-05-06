# Bevent

- InsomniaNY first [isolated the Backbone Events code](https://github.com/InsomniaNY/BackboneEvents)
- lodash is a dependancy
- I've refactored and cleaned up to satisfy Webpack/React linting in [create-react-app](https://github.com/facebookincubator/create-react-app)
- Converted to node_module format

### From node module to window global

	import Bevent from 'bevent.js';
	window.Bevent = Bevent;

### Usage

    Bevent.on('myevent', function(){
      // code
    });
    Bevent.trigger('myevent'); 
 
### Usage with payload

    Bevent.on('myevent', function(data){
      // code
    });
    Bevent.trigger('myevent', data);    


