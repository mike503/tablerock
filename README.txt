Things to keep:
- hook system
- module extensibility
- form API
- drush style management
- entity/field idea (anything and everything can be a first-class citizen, and reference each other)

Things to improve:
- everything use .php extension (no more webserver "blocking" having to happen)
- file API
- cron access
- "Content Type" -> "Entity" management

Things to reduce:
- decrease file i/o
	- less includes
	- less file scanning "magic" - heavy caching
- build-in modules - slimmer micro-kernel

Things to remove:
- all objects (especially when it is only attributes)
	bad: ->
	bad: ::
- all OO

Standards:
- no PHP 5.3 specific code
	- no namespaces
	- no "short array" syntax
- no OO code
- whitelist of "allowed" PHP functions
