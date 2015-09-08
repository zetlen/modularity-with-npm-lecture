### Modularity with NPM

The Web. The application platform of the 21st century. How everyone uses computers. (facebook, instagram, buzzfeed, tumblr, cnn, google maps, sonic fanart)

#### The Web Wasn't Supposed To Do This
 - HTML was modeled metaphorically on books. It added hyperlinks to them, but it's still designed for technical books and academic papers.
 - Don't believe me? It's got separate tags for citation (&lt;cite&gt;) and definition of terms (&lt;dfn&gt;)
 - Sure, it had some cute interactivity and presentation features. A little CSS for primping your text, a little JS for making it bounce up and down. And a blink tag.
 - We now use the Web as a full-featured application platform, on which we've standardized most of the world's consumer computing and an increasing amount of its business computing UIs.
 - This is like building a city of skyscrapers based on pop-up book technology.
 - But we did it, and it works. *We're awesome!*
 - Still...to work real well, we need to add some features to it that make it robust.

#### Modularity
 - If your whole website is one big piece, then when anything breaks, the whole thing's broken.
 - Good machines have parts you can swap out. In order to build a machine this way, you have to think about each part's inputs and outputs, its role, its purpose.
 - How would you describe what this code does, without talking about the system that surrounds it?

#### Components on the Web
 - There has to be some kind of standard system for declaring, packaging, and distributing individual components of Web functionality.
 - This isn't news to us. We've been talking about it for a decade!
 - Isn't this just "partial templates"? Isn't this just "additional stylesheets"? Isn't this just "jQuery plugins"?
 - Isn't this just "files"?
 - No. Pieces of Web functionality are too often split across several files. We have to have an intermediary step between "files", and "your whole frontend project".
 - jQuery plugins sometimes want you to download and add their CSS files, paste in particular HTML, make sure the right jQuery version is loaded first...
 - jQuery plugins are always breaking all the time
 - COINCIDENCE?
 - Something has to manage these things automatically, understand versions and dependencies, and install all the components, in the right order, to make a working machine.
 - Software package managers have been around for four Batmans.
    - apt-get, rpm, yum, fink, ports, homebrew, chocolatey
    - CPAN, Maven, Composer, RubyGems, EasyInstall, NuGet, npm
 - Like social networks, package managers are only useful if everyone is using them, so one of them has to win
 - Here are some contenders!
     - component -- abandoned!
     - jspm.io -- too new and ES6-dependent!
     - duojs.org -- too weird!
     - jam -- not well used?
     - spmjs.org -- is this only for alibaba developers?
     - bower -- now THAT'S interesting.
