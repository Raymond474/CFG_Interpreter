# Interpreters
These parsers follow different production rules, checking the input's validity.

## sp.py
This parser follows these grammar rules:
```
Grammar:
   <S> -> <A><C>
   <A> -> 'a''b'
   <C> -> 'c'<C>
   <C> -> 'd'

```
<br>
Screenshot results from my command prompt:

![Shows correct results of code running in the command prompt. Such as accepting 'abcd' and detecting 'abdd' as incorrect](images/spResults.png)

## p1.py
This parser checks if the input is a proper print statement similar to the Python interpreter.

<br>
Screenshot results from my command prompt:

![Shows correct results of code running in the command prompt. Such as accepting 'p1.in' and errors in the other input files](images/p1Results.png)

## parser2.py
This parser sollows these grammar rules:
```
Grammar:
<S> -> 'a' ( B | C ) 'd'          { 'a' }
<B> -> b                          { 'b' }
<C> -> c*                         { 'c' , 'd' }
```
<br>
Screenshot results from my command prompt:

![Shows correct results of code running in the command prompt. Such as accepting 'ad' and detecting 'abc' as incorrect](images/parser2Results.png)
