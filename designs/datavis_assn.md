---
layout: page
title: Design for Understanding
exclude: true
---

- **Group size:** Assigned teams of 4
- **Demo Day:** 2/21 _in class_
- **Design Doc Due:** 2/26, 12pm


## Overview
Mapping data to visual features is a powerful method for communicating information by leveraging the rapid perceptual pathways in our brain.  In this design sprint, you will use visual methods to communicate data - but for different end goals. Your job is to use two different lenses to approach the same dataset:

- **Clear communication and reasoning:** In this framing, you can assume that you have the user's attention and that they do not need training in traditional charts. Use your knowledge of perception + data representation to construct a series of graphs that give an in-depth, unbiased, clear portrait of your data.

- **Persuasive communication and storytelling:** In this framing, your goal is to represent the data (visually, through audio, through interaction) in the most _compelling_ way possible. What will have the most long-lasting impact on users? What will they _remember_?

Since you'll be working in teams of four (4) for this project, I recommend that you split your team into pairs. However, depending on your design, you may choose to allocate your resources in the way you see best.

### Choose a Dataset
Before you begin, choose a dataset. While you may use any dataset, be aware that cleaning the datasets into a usable format can be a major headache. Here are a few sources in which you may find data... but look for something that interests you!
<!-- - [_CORGIS (The Collection of Really Great, Interesting, Situated Datasets)_](https://think.cs.vt.edu/corgis/): cleaned, well-organized datasets that should be very simple to load into your program. -->
- [_Datasets underlying FiveThirtyEight stories_](https://github.com/fivethirtyeight/data): Mostly cleaned, but may come in different formats.
- [_Data is Plural newsletter_](https://docs.google.com/spreadsheets/d/1wZhPLMCHKJvwOkP4juclhjFgqIY8fQFMemwKL2c64vk): fascinating datasets, but may not be cleaned/curated

**Do something interesting!** I implore you to choose a topic that you find interesting and to dig into it. In the past, I've found that students sometimes gravitate towards the first cleaned data that they find. Don't let this limit the value of your output. What is a story that is _worth telling_ with data? What is a story that _people should see_ related to data?

### Your Technology
There are a wide variety of data visualization tool you can use. Personally, I find p5js a joy for creative, expressive content (and we may use it again later in the semester)... but feel free to use whatever accomplishes your goals.

- [**d3js**](https://d3js.org/): Probably the most popular data visualization library that is both powerful and flexible. However, it also has a steep learning curve - especially for people who are not comfortable with javascript and web programming. Given the very short timelines of our projects, I would only go this route if you have someone very skilled in web development on your team.

- [**Vega**](https://vega.github.io/vega/) or [**Vega-Lite:**](https://vega.github.io/vega-lite/) These are both templating tools that sit on top of the d3js visualization library. While they are less expressive than d3js, they will allow you to rapidly (hopefully) construct data visualizations. Vega will allow you to be a little more creative and integrate interaction (_recommended_).

- [**Chart.js**](https://www.chartjs.org/): a javascript library that supports easy creation of basic chart types. This will limit your flexibility, but if you want to use basic charts, it's a quick way to get rolling.

- [**P5js**](https://p5js.org/): p5js is an expressive, accessible javascript library that enables pixel-level control. While it is more difficult to construct basic charts than vega or vega-lite, it empowers more creative interpretations of data that are either more abstract or that incorporate sound.

- [**Tableau Public**](https://docs.google.com/a/bucknell.edu/document/d/1JStkKuQePhXsmMWd1JR30zPG723nJMYpGtW5s8lJZzM/edit?usp=drive_web): heavily used in business intelligence, this is the free version that can connect to a spreadsheet/file to create data visualizations for the web.


### Your Two Portraits

- _For Clear Communication:_ You should construct a series of graphs that tell the story of the data. The properties of the data should align with your chart choice. Together, your charts (_AT LEAST_ 3) should explore the data from different perspectives. For example, [Airline on-time performance](http://square.github.io/crossfilter/). While you may not have the degree of interaction of this demo, note how it gives different perspectives of the same data.

- _For Persuasion:_ There are very few guidelines here. I would encourage you to be creative and optimize for impact. For example, here is a visual/audio interpretation of data that I created (note: you need audio): [15 Years of Mass Shootings in America](https://github.com/evanpeck/15-Years-of-Mass-Shootings-in-America).


### Your Design Process
Before you got to this class, you should have read about the [five design-sheet (FdS)](http://fds.design/) approach for information visualization. You should walk through [all five stages](http://fds.design/wp-content/uploads/2015/06/five-design-sheet-approach-JCR.pdf) of FdS. Make sure to get feedback from other students in the class as part of your design process!

> Over the course of the semester, I am going to give fewer and fewer detailed instructions about how to run your design process. This is intentional! As we become more familiar with it, I expect you to be able to apply it yourself to any new technological domain

### Build it.
Just build it. Note that you may run into tensions between your imagined visualization and the one that you have time to create. That's okay! Technical tradeoffs are a reality that any designer must encounter. Adjust your design (as needed), and be sure to discuss these tradeoffs in your design document.


## Deliverables
- As always: Your design reflection as a Medium blog post. Like the last assignment, **you do not need a demo video**. However, if your visualizations contain interactive or animated elements, those should be captured in some way - for example a gif.
  - Be sure to reflect on the contrast between the two ways you have chosen to communicate your data. There are certainly tradeoffs between the two.
- Both of your designs should be hosted with publicly accessible links. These links should be clearly included into your design reflection.


<!-- ## Some Tech Tips
Over the past summer, I had another student - Gabbi LaBorwitt ('20) - complete each of these assignments to help me determine where students might encounter problems. From this project on, I will include her notes on the tech you'll be using.


### Option 1: Creating a website
_If you've never hosted a website on Bucknell's Linux servers before, here's how_

  1. On your computer open up your server space (aka your home folder) and create a folder called `public_html`
      - *MAC USERS*: If you're not using a Linux machine before beginning go to your desktop and hit `command+K` and type `smb://unixspace/linux-YOURUSERNAME.$` Once you hit enter a folder should pop-up with all of your BU Linux files
  2. In your `public_html` folder, create a second folder called `bucknell-hci`. Then, create document titled `index.html` and type something like "Hello World" inside it so we can test if it works. Afterward, you should change the name of this file to reflect what it contains.
  3. Open up Terminal and navigate it to your new folder
      - Linux Shortcut: right click on anywhere inside your folder and "Open in Terminal" should appear as one of the first options. Click that to save time navigating.
  4. In the command line type `chmod 755 index.html`
      - This changes the file's permissions to allow people from the outside see the contents.
  5. Now go online to `eg.bucknell.edu/~YOURUSERNAME/bucknell-hci/` to be able to see it.
      - Added bonus: You can use this space as personal website for the rest of your time at Bucknell, too.

### Option 2: Use a service with free web hosting  -->


------------

## Tips for Getting Data into p5js

  1. Use the [P5js online editor](https://editor.p5js.org/) editor
  2. Go through [this](https://creative-coding.decontextualize.com/first-steps/) tutorial to get a sense of what p5 is and how to use it.
  3. If you're not familiar with javascript arrays, check out [this tutorial](https://creative-coding.decontextualize.com/arrays-and-objects/)... otherwise, skip ahead to [using csvs in p5js](https://creative-coding.decontextualize.com/csv-files/).



<!-- ## Tips for Vega Lite (or Vega)

### Introducing Vega-Lite:
  1. Open up Vega-Lite's [online editor](https://vega.github.io/new-editor/?mode=vega-lite) to work out of
  2. Look through the charts and graphs we're given (found in the dropdown menu) to see the different possibilities for visualizing data with Vega-Lite.
  3. Go through their first two [tutorials](https://vega.github.io/vega-lite/tutorials/getting_started.html#embed) titled "The Data" and "Encoding Data with Marks". Code along with the tutorial in order to get a better feel for the library. Some helpful tips:
      1. Entire code should be wrapped in `{}`.
      2. Almost every value you enter must be wrapped in `""`– excludes punctuation and numerical values in the `data: values` field.
      3. The `encoding` field is where you'll enter the bulk of the information about your dataset. Most importantly the x- and y-axis data go here. *[Learn about the different data types here](https://vega.github.io/vega-lite/docs/encoding.html#data-type)*.
      4. Create a legend using [this documentation](https://vega.github.io/vega-lite/docs/legend.html).
  4. When you're done going through the tutorial, use the data found in [this](https://github.com/plotly/datasets/blob/master/2014_apple_stock.csv) csv file to create a chart or graph.
      - To use data from an online link, replace `"data": { "values": [..] },` with <br> `"data": { "url": "URL", "format": {"type": "TYPE"} },` where `TYPE` is the type of file used (csv in our case).
      - When you're entering the x- and y-axis "fields", instead of typing `a` and `b` you'll type in the names of the columns you'd like to display the data for. In this example there are only two columns so your x field would be "AAPL_x" and your y-field would be "AAPL_y".
  5. Once you finish playing around with your chart or feel like you understand how the code works, move on to the next task.


### Publishing your Visualization:
  1. Once you're diagram is finished open the `index.html` in the `public_html` folder that you created earlier in a text editor.
  2. Delete anything that's already in the file and use the code given [here](https://vega.github.io/vega-lite/tutorials/getting_started.html#embed) (if your computer isn't already there, go to the section titled "Publish your Visualization Online") to guide you in adding your chart or graph to your webpage.
      - Don't forget to include `var vlSpec = {` before entering your diagram code as well as the optional code for vega-lite that we need `var opt = {"mode": "vega-lite"};` towards the bottom.
  3. Once completed, you should be able to see your diagram -->
