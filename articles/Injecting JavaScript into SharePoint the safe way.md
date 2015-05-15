# Injecting JavaScript into SharePoint the safe way
Use namespaces in order to avoid conflicts of your JavaScript customizations with standard SharePoint JavaScripts and customizations deployed by other developers. 

 **Last modified:** April 30, 2015

 _**Applies to:** apps for SharePoint | SharePoint 2013 | SharePoint Online_

**In this article**

[Why this is important](#sectionSection0)

[How to use namespaces](#sectionSection1)

[OfficeDev/PnP](https://github.com/OfficeDev/PnP/) provides various samples and solutions that include JavaScript code. In order to make demonstrated techniques easy to understand, these samples are usually oversimplified and do not use namespaces when  injecting JavaScript code into SharePoint. It is important to ensure that you follow the simple steps outlined in this article when encorporating OfficeDev/PnP samples into your solutions.

## Why this is important
<a name="sectionSection0"> </a>

JavaScript is a loosely typed language. If you define a variable or function, and variable or function with the same name already exists in the current context, the new value or implementation will replace existing one.
As a result, when injecting JavaScript code into SharePoint it is easy to override standard SharePoint JavaScripts or customizations deployed by other developers.
This may lead to conflicts that may be hard to identify and debug.

In order to avoid such situations it is recommended that you always use custom namespaces for your JavaScripts.

## How to use namespaces
<a name="sectionSection1"> </a>

The sample below demonstrates a simple pattern used to organize JavaScript code in namespaces and classes.

```JavaScript
var MySolution = MySolution || {};

MySolution.MyClass1 = (function () {
    // private members
    var privateVar1 = 1;
    var privateVar2 = 2;
    
    function privateFunction1(){
      return "";
    }
    
    return {
        // public interface
        myFunction1: function() {
          return privateVar1;
        }
        myFunction2: function(){
          return privateVar2;
        }
    };
})();
```

Functions defined in public interface can be invoked as:
```JavaScript
MySolution.MyClass1.myFunction1();

MySolution.MyClass1.myFunction2();
```

This allows you to avoid naming conflicts with standard SharePoint JavaScripts and customizations deployed by other developers as now all your code uses custom *MySolution* namespace.
