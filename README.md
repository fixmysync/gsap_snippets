#GSAP Snippets
#### Quick + Easy Code Completion for the GreenSock Animation Platform

Type the snippet shortcode and then press Tab to complete the snippet.

The snippets are listed below in alphabetical order. The '`{$1}`' indicates the initial position of the caret. Some snippets have multiple tab-stops, as indicated by '`${2} ${3} ${4}`' where the number is the order in which you tab through the snippet.

Feel free to play with, alter, expand, or do what you want with these snippets. If you come up with a very useful snippet, or a mistake or simply something that I have missed - Please let me know (via [Twitter](https://twitter.com/mandymadethis), [GitHub](https://github.com/MandyMadeThis) or as a comment on the original [blog post](http://mandymadethis.com/sublime-text-gsap-snippets/)) so that I can improve these for everybody. Thanks!

*note*: I use `TimelineMax` most of the time and I chain my tweens directly to the timeline.   
Example:   

    var exampleTL = new TimelineMax()
        .staggerFrom(["h1, h2, button"], 0.5, {y:100, autoAlpha: 0, ease: Power3.easeOut }, 0.25)
        .staggerFrom(".myClass", 0.5, {x: -200, autoAlpha: 0, ease: Power3.easeOut }, 0.2, "-=0.5")
        .to("#myID", 1, {y: 85, ease: Power3.easeInOut})
        .to(".element", 0.5, {opacity: 0.3 }, "-=0.5");


This is why I have included the `.` before most of the tweens, but I've not included a `;` at the end of them. Please feel free to adjust these and make them work for your own GSAP code style.       

**Draggable**   
`Draggable.create(${1:element}, {type: "${2:drag_type}", ${3:vars}});`      
  
---   

**from**     
`.from(${1:element}, ${2:1}, {${3:vars}, ease: ${4:Power3.easeInOut}})`      

---   

**fromTo**  
`.fromTo(${1:element}, ${2:1}, {${4:fromVars}}, {${5:toVars}})`   

---   

**set**  
`.set(${1:element}, {${2:vars}})`   

---   

**SplitText**  
`SplitText(${1:element}, {type:"${2:words,chars,lines}"});`  

---   

**stagger**   
`.stagger${1:To}(${2:element}, ${3:0.5}, {${4:vars}, ease: ${5:Power3.easeInOut}}, ${6:0.25})`   

---   

**staggerFromTo**   
`.staggerFromTo(${1:element}, ${2:0.5}, {${4:fromVars}}, {${5:toVars}}, ${6:0.25})`   

---   

**Timeline**   
`new Timeline${1:Max}(${2:{options\}})`   

---   

**to**
`.to(${1:element}, ${2:1}, {${3:vars}, ease: ${4:Power3.easeInOut}})`   

---   

**Tween**   
`Tween${1:Lite}.${2:to}(${3:element}, ${4:1}, {${5:vars}, ease: ${6:Power3.easeInOut}});`


