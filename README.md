# AMDsnippets

[![Join the chat at https://gitter.im/pierceray/AMDsnippets](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pierceray/AMDsnippets?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
Sublime Text AMD Snippets

## Installation

Use Sublime Text's [Package Control](https://sublime.wbond.net/installation) to install this plugin.

## Manual Installation

Open up Terminal.app and execute these commands:

### Sublime Text 2

    cd ~/Library/"Application Support"/"Sublime Text 2"/Packages/
    git clone git@github.com:pierceray/AMDsnippets.git

### Sublime Text 3

    cd ~/Library/"Application Support"/"Sublime Text 3"/Packages/
    git clone git@github.com:pierceray/AMDsnippets.git

## Snippets
Start typing `define` and the snippets should appear in the autocomplete.

### AMD Anonymous Module
```
define( [
    '${1:dependencies}'
], function (
    ${2:DependParam}
) {
    ${2:DependParam}.${3:methodToCall}();
} );
```
### AMD Twitter Flight Module
```
define( [
	'${1:flight/lib/component}'
], function (
	component
) {
	return component( ${2:functionNameUI} );

	function ${2:functionNameUI}() {

		this.attributes( {
		} );

		this.after( 'initialize', function () {
		} );

		this.${3:methodName} = function(){
		};
	}

} );
```
### AMD Named Module
```
define(
	'${1:module_id}',
[
	'${2:dependencies}'
], function (
	${3:DependParam}
) {
	${3:DependParam}.${4:methodToCall}();
} );
```

## Usage
Tab through the snippet params and fill in your information.
