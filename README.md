## PHP advanced concepts 
### Namespaces

```
<?php
/*
 * Namespaces can be referred to as grouping which allows you to define classes and other 
 * entities under a group so that it does not conflict with  same name class in other group 
 */
namespace my\name; 

class MyClass {}
function myfunction() {}
const MYCONST = 1;
?>
```
### Inheritance using Traits
```
trait Subscriber{
    public function subscriberLogin() {
        echo "You\'re Logged in as Subscriber". '<br/>';
    }

}

trait Contributor{
    public function contributorLogin() {
        echo "You're Logged in as Contributor". '<br/>';
    }
}

use Subscriber, Contributor;

public function run() {
	$this->subscriberLogin();
	$this->contributorLogin();
}

$authentication = new Member();

$authentication->run();
```
### Interfaces & Abstract Classes
### Traits
### Class Reflection
### Inheritance Scope & Late Static Binding
### Overloading & Magic Methods

