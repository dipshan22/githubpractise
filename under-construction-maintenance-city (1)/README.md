# Under construction/maintenance city

A Pen created on CodePen.io. Original URL: [https://codepen.io/fbuireu/pen/XBGZdd](https://codepen.io/fbuireu/pen/XBGZdd).

##Under construction/maintenance city

Fully responsive minimal  "under construction" city, which became less tightened as the window width decreases. It's a pure SCSS pen, no JS has been used.

The HTML uses two mainly `<section>` in order to separate the text and the city. The first one doesn't have much mystery; it's just a simply `flexbox`. The second one stands for the city stuff; internally it's just nested `<ul>` and `<li>` structure. I've decided to use this structure because it turns easy to imagine what's inside each list. 
In detail, the main `<ul>` represents the city cranes, buildings and trees, with all necessary parts inside (cables, cabin, arm, weight for cranes and tree and trunk for trees).

Regarding the SCSS, the interesting part in this pen, it's based in BEM methodology and it has been enriched with some useful key comments. I've used a SCSS loop to build each part (buildings, cranes and trees), including some conditions inside to shape the positioning of and detailing specific items. This is also useful to remove them in the responsive scenario and to add some delay between animations. 

* Buildings are made using a `data-image` background which is repeated (represents the windows) and a gradient which represent a shadow.

* Cranes, the tricky part, are made using a coordination of animations, translating and changing the height of the hook. And changing the `perspective` property of the cables and other items to make the crane turn effect. There's only one SCSS crane constructor, the other cranes are made modifying the `scale` (and `scaleX`) properties. I've also played with the `z-index` property to put them at the desired depth.

* Trees are made using the `border` property, simulating a pine tree (which it's easier than others) also playing with them depth. I've also changed the `border-left` color to simulate a shadow, as I did with the buildings.

---

**Acknowledgements:** Marian Alrt ([@marianarlt](https://codepen.io/marianarlt))  for the [idea, crane and building construction](https://codepen.io/marianarlt/pen/NxWXXd).