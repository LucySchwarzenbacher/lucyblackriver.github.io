---
title: Button
info: Use buttons to signal actions.
nav: true
---

# Main Buttons

The main buttons in our application are used to login/logout and for the uploadform. Because Ruby on Rails mainly uses the button-tag to send a form, we used a link-tags most of the time and gave them the button styles.

{% include pattern_block.html url='/src/patterns/components/button/default_button.html' %}
{% include pattern_block.html url='/src/patterns/components/button/disabled_button.html' %}

A button can be disabled, pointer events will not occur.


# Ghost Buttons

The ghost buttons are used in smaller elements of our application. For example to show idividual challenges or posts, or as a link to another page of the project. Like we did with the main buttons, we also mainly used link-tags and styled them accordingly. The only time we used a button-tag was on our filter-form.

{% include pattern_block.html url='/src/patterns/components/button/default_ghost_button.html' %}
{% include pattern_block.html url='/src/patterns/components/button/disabled_ghost_button.html' %}

