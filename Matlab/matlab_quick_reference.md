# Content Table 
* [Intro](#intro)
* [Conmand Window](#command-window)
* [Data](#data)
* [Control flow](#control-flow)
* [Method and function](#method-and-function)
* [Class](#class)
* [Package](#package)
* [Input and output](#input-and-output)
* [Error and Exception](#error-and-exception)
* [Coding style](#coding-style)
* [Libraries](#libraries)
* [Arithematic calculation](#arithematic-calculation)

# Intro 
<a name= "#intro"></a>
> Replace this line with the introduction

# Command Window
<a name = "command-window"></a>

# Data 
<a name= "#data"></a>

## **Example Code**

## **Primitive Data**
### int

### float

### double

### operators

### convertion

## Boolean

## Character

## String

## **Array**

## **List**

## **Set**

## **Enumerat**

## **Structure**


# Control flow
<a name= "#control-flow"></a>

## **if...else**

## **while**

## **for**

## **switch**

## **try...catch**
```MATLAB
% Catch error and display a warning
try
    a = notaFunction(5,6);
catch
    warning('Problem using function.  Assigning a value of 0.');
    a = 0;
end

% Catch error and add discription
try
   C = [A; B];
catch ME
   if (strcmp(ME.identifier,'MATLAB:catenate:dimensionMismatch'))
      msg = ['Dimension mismatch occurred: First argument has ', ...
            num2str(size(A,2)),' columns while second has ', ...
            num2str(size(B,2)),' columns.'];
        causeException = MException('MATLAB:myCode:dimensions',msg);
        ME = addCause(ME,causeException);
   end
   rethrow(ME)
end 
```



# Method and function
<a name= "#method-and-function"></a>

## **Example Code**


# Class
<a name= "#class"></a>

## **Example Code**
```MATLAB
classdef(Attribute) ClassName
% Class Name    Summary of the class
%   Detailed explanation

    properties(Attribute)
        property1   % Explanination for property 1
        property2   % Explanination for property 2
    end

    methods(Attribute)

        function obj = ClassName
            % Summary of the constructor

        end

        function out = functionName(in)
            % Summary of the function
        end
    end

    events(Attribute)

    end

    enumeration(Attribute) % Why it is not blue?

    end
end
```
**Note:**
* Attribute is optional.
* Use ```doc ClassName``` to show the documentation.


## **Properties**

## **Methods**
```MATLAB
methods
    function obj = ClassName()
    % This is the constructor methods
    % It has to have a obj object
    end
end

methods(SetAccess = public)
    function out = publicMethod(in)
    % This is a public method
    end
end

methods(SetAccess = private)
    function out = privateMethod(in)
    % This is a private method
    end
end

methods(Static)
    function out = staticMethod(in)
    % Use static method to set static variables
    % This works like a seter and getter function
        persistent val
        if nargin
            val = in
        end
        out = val
    end
end
```

## **Events**

## **Enumeration**


## **Override methods**

## **Inheritance**

## **Others**

# Package
<a name = #package></a>

# Input and output
<a name= "#input-and-output"></a>

# Error and exception
<a name= "#error-and-exception"></a>


# Coding style
<a name= "#coding-style"></a>


# Libraries
<a name= "#libraries"></a>

# Arithematic calculation
<a name= "#arithematic-calculation"></a>