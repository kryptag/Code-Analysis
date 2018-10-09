### Report

Using [graphql-jpa](https://github.com/jcrygier/graphql-jpa)

#### CouplingBetweenObjects
Reason why i picked this whas because this is because Low coupling and high Cohesion has become the mantra for software development. And that is because of the strength that it brings to development, if you follow this design pattern you will find that changed out components, extending or implementing other classes or interfaces becomes a breeze. 

#### SwitchStmtsShouldHaveDefault
A switch statement should always have a default value or else you will have values that will not hit a single case and just fall through. This will cause issues because you will have certain outcomes that won't trigger anything.

#### AvoidDeeplyNestedIfStmts
This more or less explains itself, the big issue with having deeply nested if statements is that you raise complexity and coupling. This also makes testing an impossible task, because for each nested case you need to test a new code branch. 

#### AvoidThrowingNull
This is more or less the golden rule in Java and should not be taking lightly, null has a lot of usages in programming, but throwing null can be a nightmare for your application. If this is not handled and caught in the right layer this will bubble up and can end up crashing your application

#### CyclomaticComplexity
This has a lot in common with "AvoidDeeplyNestedIfStmts" as by having a lot of if statements will raise the CC. Cyclomatic Complexity is the measurement of all the linear indepentend paths through a method or function. 

#### LogicInversion
By example, instead of testing if all elements in list upholds a predicate you should rather test for the ones that don't. And if your goal is to have all elements in that list to uphold the predicate then you want to use the logic above. This will give you a better run time when it comes to performance but make the logic comprehension easier. 

#### SimplifyBooleanReturns
This is one of the points that comes down to readability, instead of having 
```
if(a == b) then return true
or return false;

you can do 

return a == b;
```
This makes the method more simple and exactly explains what is happening in the one method.

#### BadComparison
We should not compare volatile types, in this case that would be Doubles because the precision when comparing floating point. And this is very likely to cause problems or inconsistencies when doing logical operations

#### NullAssignment
This comes down to the idea that you don't want to assign variables to null after they have been instatiated, by doing this you will increase the chance of errors. And you can have problem with returning null. 

#### UseArrayAsList
This is something that can be horrible for your application performance. This method should be used when you want to copy an array, this method copies the array and all its elements. Instead of doing a foreach where you loop through every element and copying it 1 by 1. 


#### Performance
I tried for a long time to get this up and running, Couldn't get Netbeans profiler to work.
