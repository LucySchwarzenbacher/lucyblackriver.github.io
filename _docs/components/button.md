---
title: Button
info: Use buttons to signal actions.
nav: true
---
The application ColourInstinct is set up with Ruby on Rails. Since this framework implements the `button`-tag to send a form, we oftentimes opted for `a`-tags and applied the corresponding button styles.

In the examples below, the first button is an `a`-tag, the second is a `button`-tag.

# Main Buttons

The main buttons in the application can be found in the login/logout section and the upload form. For the login/logout buttons we used `a`-tags, for the form we used the `button`-tag.

{% include pattern_block.html url='/src/patterns/components/button/default_button.html' %}

When you hover over the main buttons with your mouse, their size will increase and the mouse pointer will change to indicate that they are clickable.

{% include pattern_block.html url='/src/patterns/components/button/disabled_button.html' %}

If the buttons are disabled, their colour changes to gray and no hover or pointer event will occur.


# Ghost Buttons

The ghost buttons are used for smaller elements in the project, e.g. to show idividual challenges or posts, or as a link to another page of the application. Like we did with the main buttons, we also mainly used `a`-tags and styled them accordingly. The only time we used a `button`-tag was on our filter form.

{% include pattern_block.html url='/src/patterns/components/button/default_ghost_button.html' %}

The hover effect for these buttons differs from the main buttons. Instead of an altering size, the buttons adapt their background to the `$highlight` colour.

{% include pattern_block.html url='/src/patterns/components/button/disabled_ghost_button.html' %}

The disabled ghost buttons have the same characteristics as the main buttons, which means background is coloured gray and no hovor and pointer events occur.

