# bulma-slider
Bulma's extension to display sliders
(find all my bulma's extensions [here](https://wikiki.github.io/bulma-extensions))

<img src="./slider-example.png" width="100%">

Usage
---

```html
<input class="slider" min="0" max="100" value="50" disabled="" type="range">
```

Modifiers
---
This extension uses Bulma's color & size modifiers

You can also use ```is-circle``` modifier on slider to get a circle thumb and ```is-fullwidth``` to get a fullwidth slider

Variables
---
Name | Default value    
-----|---------------
$slider-radius | $radius
$slider-track-background | $grey-light
$slider-thumb-background | $primary
$slider-track-radius | $radius
$slider-thumb-radius | $radius

Demo
---
You can find a demo [here](https://codepen.io/wikiki/pen/gxKgEO)

Integration
---
- Clone the [bulma repo](https://github.com/jgthms/bulma)
- Under the `sass` folder, create a new folder called `extensions`
- In this new folder, create a new file `clliser.sass`
- Copy the code form the `bulma-cliser repo`'s [cliser.sass](https://github.com/Wikiki/bulma-cliser/blob/master/cliser.sass) file into your new file
- In the same folder create a new file `_all.sass` (this is not required, but will help when you add more extensions)
- In this file add this code:
```
@charset "utf-8"
@import "cliser.sass"
```
At the end of the `bulma.sass` file, add this line: `@import "sass/extensions/_all"`

Now, you can just build the bulma project with `npm run build`, and the output will be available in the `css folder`.
