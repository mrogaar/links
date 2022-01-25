# Links

448 hand-picked tools & resources for web designers & developers.
https://toolkit.addy.codes/

Array cheatsheet.
![image](https://user-images.githubusercontent.com/47871735/124391730-456e8780-dcf2-11eb-92af-69075c4e4c7d.png)

# Links voor Oxygen

Hoverify browser extension

Hydrogen Pack

https://editorenhancer.com/pricing/

Oxy Toolbox

ACF Tools

WP Gridbuilder

Swiss knife oxygen builder

https://www.youtube.com/watch?v=hCYJgAVeBN8


# Responsive font calc:

```scss
// Fluid typography calculator
// Usage: fluid($min, $max)
// $min and $max without rem
// html font size 62.5% 
$viewportmin: 37.5;
$viewportmax: 124;
@function fluid($min, $max) {
    $minrem: $min * 1rem;
    $maxrem: $max * 1rem;
    $viewportminrem: $viewportmin * 1rem;
    
    $XX: $viewportminrem / 100;
    $YY: 100 * ($max - $min) / ($viewportmax - $viewportmin);
    @return clamp(#{$minrem}, calc(#{$minrem} + ((1vw - #{$XX}) * #{$YY})), #{$maxrem});
}

```
