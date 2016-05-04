Sticky Layout
====
A simple set of CSS rules to turn the main HTML file into a centered 3 column layout with sticky header and footer.


Usage
----
The simplest implementation is to create a `#stky-body` element between two `.stky-row` elements. 
There can only be one `#stky-body`, but multiple `.stky-rows`. 

```
<div class="stky-row"></div>
<div class="stky-body"></div>
<div class="stky-row"></div>
```

You can also have a responsive center column (snaps to 1170 > 970 > 768px):

```
<div class="stky-row"></div>
<div class="stky-body">
    <div class="stky-container"></div>
</div>
<div class="stky-row"></div>
```

and even columns within that (default at 200px | 200px | 100%-400px):

```
<div class="stky-row"></div>
<div class="stky-body">
    <div class="stky-container">
        <div class="stky-columns">
            <div class="stky-left"></div>
            <div class="stky-center"></div>
            <div class="stky-right"></div>
        </div>
    </div>
</div>
<div class="stky-row"></div>
```

If having a three column layout is too restrictive, you can resize any two or use a full width one:

```
<div class="stky-row"></div>
<div class="stky-body">
    <div class="stky-container">
        <div class="stky-columns">
            <div class="stky-full"></div>
        </div>
    </div>
</div>
<div class="stky-row"></div>
```

If you are already using a library like Bootstrap, you can replace `.stky-container` with Bootstraps `.container` 
and use all the `.row` and `.col-*` columns however you want. You can even use the `.container` class within the 
header or footer elements to keep everything on a resize grid, but still have full width header, nav and footer rows.





