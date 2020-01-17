# terseStrap

## V 0.1.2 Not ready for mass consumption
 TerseStrap is a collection of .SCSS utility classes based on common CSS rules that I find myself reusing.

 Frustrated with lack of multi-language auto completion support for common BS4 classes, I set out
 to make a terse set of utility based atomic classes.


## Important note about IE support
 Don't count on it! I'm not jumping thru hoops to support an outdated browser.


## Design Philosophy
 The classes I've created generally follow a property - value approach.
 e.g. `.ta-l = text-align (property), left (value)`


 Some classes provide multiple options.
 
 Consider the following:
 - `.ai-s--jc-s` for a relatively long class (align-items-start--justify-content-start)
 - `.ajs` for the tersest class (alignitemsjustifystart)
 Both of the above classes provide the same css declarations:
 ```
 align-content: flex-start;
 justify-content: flex-start;
 ```

## Project goals
 Eventually I want to turn this into an easily accessible npm package.


## Contributing
 Fork the repo then submit a PR.
 Raise an issue and I'll check it out.