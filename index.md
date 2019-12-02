---
layout: plain
title: Documentation
---
Editing the WAND site
=====================
- - -

## Adding a main page
To add a main page, simply add the markdown file to the site's main directory. To add a link to it in the nav bar, add its address to the `data/navigation.yml` file.




## Using the different layouts

**default** - Will simply output the content unformatted and center aligned. This layout it designed as a gateway for other layouts and so I would not recommend using it for content directly.

**maps** - Outputs the content in a div 40% of the page width, leaving space on the right for a google maps embed.

**people** - Any content will be output normally. Then a list of the people in the peoples collection will be output and formatted in a tidy manner.

**person** - Name and role values will be displayed next to an image that's src is derrived from the image name. Any input content will then be attached below this, followed by a table of projects that have been listed in the person's front matter.

**plain** - Outputs the content as plain text aligned to the left.

**project** - Output content as plain text, then attach a link back to the topic the project is related to.

**research** - List all the items in the research collection each with a link to their respective topics and set every second ones color to off-white.

**sections** - Split the content based on input `<!--split-->` tags. Then set every second section to off white.

**topic** - Display input content and then list all projects associated with the topic in a table.

**twitter** - Similar to maps, output the content to fill 60% of the display width and then attach a twitter scroll to the right side of the content.