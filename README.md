# About

This is a candidate for the reference javascript implementation of the [Porter2 stemming algorithm](http://snowball.tartarus.org/algorithms/english/stemmer.html), 
(rev. July 2005).


There is a second project which covers the [original Porter Stemmer from 1980](http://tartarus.org/martin/PorterStemmer/def.txt), 
you can find that at the following url: https://github.com/kristopolous/Porter-Stemmer.

The reference has also been included in the spec directory.

# Usage

Include the js file, then run `stemmer(<word to stem>)` to return the stemmed word.

You can get a trace as to what is going on, corresponding to the steps outlined in the papers, by provding a second argument of "true" 
and using one of the browser debug consoles. 

For instance, `stemmer("hopefully", true)` will output `1c /^(.*[aeiouy].*)y$/ hopefulli`, telling us that rule 1c was matched
by that regular expression and as a result, we got hopefulli.

# Status

As of Oct 22, 2012, PorterStemmer2 is 98.54% compliant.

