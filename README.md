# **sailsInfo** for V.0.9.*

Basic Information and Cheat Sheet for Sails.js

## Controller default actions
Change "Model", "models", "model" to fit your Model name.
```javascript
module.exports = {
	index: function(req, res) {
		Model.findAll(function(err, models){
        	res.view({models: models})
        })
	},
    
    show: function(req, res){
    	Model.findOne(req.param('id'), function(err, model){
        	res.view({model: model})
        })
    }
};
```
	

	
