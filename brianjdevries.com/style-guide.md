# Site Style Guide

<main>

## Colors

<div style="display: flex; flex-direction: row;">
  <div class="swatch" style="background-color: #e34234; color: black;">Vermillion</div>
  <div class="swatch" style="background-color: #1e1e1e; color: white; margin-left: 0.5rem;">Dark</div>
  <div class="swatch" style="background-color: #fefefe; color: black; margin-left: 0.5rem; border: 1px solid black;">Light</div>
</div>

## Demos

## Typography

### Headers and Text

<div class="demo" data-demo-label="Functions.js">
  <h1>Top Level Header</h1>
  <h2>Second Level Header</h2>
  <h3>Third Level Header</h3>
  <h4>Fourth Level Header</h4>
  <h5>Fifth Level Header</h5>
  <h6>Sixth Level Header</h6>
</div>

### Links

### Blockquotes

## Web Fonts



## Code Blocks

## Icons

## Lists

## Comments?

## Tables

## Fluid Media

## Other components

- [x] Colors
- [ ] Demos
- [ ] Typography
  - [ ] Headers and Text
    - [ ] h1, h2, h3, h4, h5, h6
    - [ ] Primary Title
    - [ ] Links
    - [ ] blockquotes
- [ ] Web Fonts
- [ ] Code
  - [ ] Inline
  - [ ] Block
  - [ ] > Use_Prism.js?
- [ ] Icons
- [ ] Lists
  - [ ] Ordered
  - [ ] Unordered
  - [ ] Description
  - [ ] Inline
  - [ ] Posts List
- [ ] Comments?
  - [ ] Nested replies
- [ ] Tables
- [ ] Fluid Media
  - [ ] Image
  - [ ] Full width image
  - [ ] Video
  - [ ] Third party video
  - [ ] Figure with caption
  - [ ] Standalone caption
- [ ] Other components
  - [ ] Fixed table of contents
  - [ ] Printed page
  - [ ] Callout
    - [ ] Update
    - [ ] Warning

</main>

<style>
  main {
    font-family: Georgia,serif;
    font-size: 1rem;
    line-height: 1.2rem;
  }

  h1,h2,h3,h4,h5 {
    font-family: arial,Helvetica,sans-serif;
  }

  .swatch {
    max-width: min-content;
    padding: 0.5rem 1rem;
    border-radius: 0.25rem;
  }

  .demo {
    position: relative;
    padding: 0.75rem;
    /* border: 2px solid #e34234; */
    border-radius: 0.5rem;
    box-shadow: 0 0 0 var(--box-shadow-width,2px) #e34234;
  }

  .demo::after {
    content: "Demo";
    position: absolute;
    right: 1rem;
    top: -0.45rem;
    font-size: .8rem;
    padding: 0 .25rem;
    line-height: 1;
    background: #fefefe;
    color: #e34234;
  }

  .demo[data-demo-label]::after {
    content: attr(data-demo-label);
}

</style>