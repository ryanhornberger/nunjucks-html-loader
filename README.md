Nunjucks (Webpack) HTML Loader
-----------------------

This is a webpack loader that takes nunjucks templates and returns raw html. It also works with webpack's watch command

Contributing
------------

Submit a pull request. I'll get to it when I get time

Licensing
---------

MIT

Usage
-----

	{
        test: /\.nunj$/,
        loader: 'file?context=' + precompiledContext + '&name=[path][name].html!nunjucks-html?' +
        	JSON.stringify({
        		'searchPaths': [
					'/path/to/sources',
					'/path/to/more/sources'
				]
        	})
    }