---
title: Class Naming Conventions
info: Class Naming Conventions used in this system.
---

# BEM
Generally speaking, classes and identifiers in the project are in lowercase and english. Furthermore, the classes are declared according to the the BEM pattern. In other words, a class name follows the block__element-modifier syntax. This is not only helpful to establish a clear structure and hierarchy, but also assists in writing clean and tidy (S)CSS code. 

BEM is a component-based approach that divides the interface into independent blocks. The name of a BEM entity is unique and equal throughout the used technologies (CSS, JavaScript and HTML). The goal of the given names is to inform the developer about their content.

Rules that are considered in the project:
* names in lowercase 
* if a block is described by more than one word, use `-`
* if a block is modified, use one underscore (`_`) between words
* the element name is separated from the block name by double underscore (`__`)
* the modifier name is separated from the block name or element name by double dash (`--`)

**More information about BEM:** http://getbem.com/introduction/  
**More information about Code Conventions:** https://en.bem.info/methodology/naming-convention/

## Block
### Naming
Block names are in lowercase. If block is described by more than one word, use `-`. If a block is modified, use one underscore (`_`) between words. A prefix needs to be added to form a CSS class.  

**Example:**
> `.block`

### HTML
If DOM node accepts class name, it can classify as a DOM node.
```/
<div class= "challenge">
    . . .
</div>
```

### CSS
The DOM node is used with class name selectors only.
```/
.challenge { 
    color: $white 
}
```

## Element
The elements are tied to its block and have no standalone meaning.

### Naming
The element name is separated from the block name by double underscore (`__`)

**Example:**
> `.block__elem`

### HTML
If an element is within a DOM node, it can be declared as an element.
```/
<div class="challenge">
    <div class="challenge__item>
        . . .
    </div>
</div>
```

### CSS
The element is used with class name selectors only with no dependency to other blocks.
```/
.challenge__item { 
    color: $white 
}
```

## Modifier 
They are used to describe the appearance, behaviour or state of blocks.

### Naming
They consist of the elements's or block's ame with two dashes that describe the given appearance, behaviour or state. The modifier name is separated from the block name or element name by double dash (`--`)

**Example:**
> `.block--mod` // `.block__elem--mod` 

### HTML
They are added as an extra class to the DOM node, while still using the original class.
```/
<div class="challenge">
    <div class="challenge__item--active>
        . . .
    </div>
</div>
```

### CSS
The modifier class name is used as a selector.
```/
.challenge__item--active { 
    color: $white 
}
```
**Inspired by:** http://getbem.com/naming/

