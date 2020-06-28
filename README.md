# terseStrap

## V 0.5.0 Experimental.
 TerseStrap is a collection of .SCSS utility classes based on common CSS rules that I find myself reusing.

 Frustrated with lack of multi-language (e.g. JSX, twig etc.) auto completion support for common BS4 classes, I set out to make a terse set of utility based atomic classes.

## Requirements
- An SCSS compiler.


## Important note about IE support
No IE support.


## Design Philosophy
 The classes I've created generally follow a property - value approach.
 e.g. `.ta-l = text-align (property), left (value)`

 Some classes provide multiple options.
 
 Consider the following:
 - `.ai-s--jc-s` for a relatively long class (align-items-start--justify-content-start)
 - `.ajs` for the tersest class (alignitemsjustifystart) very dense, only 3 key strokes.
 Both of the above classes provide the same css declarations below:
 ```
 align-content: flex-start;
 justify-content: flex-start;
 ```
 These two classes are simply different ways to make the same declarations, one is slightly more readable, the other terser. There are many instances of classes like this.
 
**Is this readable?** Probably not. Make sure you document usage of this library in your project documentation so people don't freak out. Once you understand what these classes are saying, it's fairly self evident in what they are accomplishing.


**Why do I need this library with component based development?**
Some styles in components violate DRY. All tersestrap classes are usable over a whole project.There is no need to ever write "display: flex; justify-content: space-between;" in your component because I guarantee you that will be used somewhere else in a decently sized project.

While CSS in JS is fine, CSS still has an important place in modern web development.


## Project goals
- Turn this project into an easily accessible npm package.
- Create a small documentation website to list classes (similar to bootstrap)
- Potentially create terse responsive classes. These will follow bootstrap media query sizes. In future I'll provide documentation to make it easy for users to adjust for their own breakpoints widths (however these will follow bootstrap style class breakpoints e.g. md, lg etc).


## Contributing
 Fork the repo then submit a PR.
 Raise an issue and I'll check it out.


## Changelog (starting 0.4.0):
`Version 0.5.0:`
- Removed "optional boilerplate" files. The goal of this project is to allow anyone to drop in these classes without worrying about compatibility or having to override anything with their own classes. This project is about universal plug and play, not reconfiguring or restyling (think bare bones, let the designers do their thing and let the devs save on some key strokes, no fighting with this library ever needed).
- Confirm NO support for IE moving forward (ever).
- Confirmed with NPM that scss packages are ok (it doesn't have to be a JS project).
- Refined (based on the above point) project goals. Added new goals to push usable release out faster. Future responsive classes will be backward compatible.
- Confirmed importance of project (i.e. why use it).
- Add requirements as tersestrap will certainly use SCSS. TerseStrap will never rely on another library, outside of referring to popular conventions found in other libraries (especially bootstrap).

`Version 0.4.0:`
 - Adjusted versioning to better match `semver.org` (currently no hotfixes have been made, only backward compatible updates)
 - Added optional boilerplate