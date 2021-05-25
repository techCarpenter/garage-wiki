# Site Style Guide

<main>

## Colors

<div style="display: flex; flex-direction: row;">
  <div class="swatch" style="background-color: #e34234; color: black;">Vermillion</div>
  <div class="swatch" style="background-color: #1e1e1e; color: white; margin-left: 0.5rem;">Dark</div>
  <div class="swatch" style="background-color: #fefefe; color: black; margin-left: 0.5rem; border: 1px solid black;">Light</div>
</div>

## Demos

<div class="demo">
  <p>This is a basic demo</p>
</div>

<div class="demo" data-demo-label="New label">
  <p>This is a demo with a new label.</p>
</div>

## Typography

### Headers and Text

<div class="demo">
  <h1>Top Level Header</h1>
  <p>This is a paragraph to give sense of the flow of a document that has headers. There shouldn't be a huge gap around the headers, but enough to make text readable and let the headers stand out!</p>
  <h2>Second Level Header</h2>
  <p>This is a paragraph to give sense of the flow of a document that has headers. There shouldn't be a huge gap around the headers, but enough to make text readable and let the headers stand out!</p>
  <h3>Third Level Header</h3>
  <p>This is a paragraph to give sense of the flow of a document that has headers. There shouldn't be a huge gap around the headers, but enough to make text readable and let the headers stand out!</p>
  <h4>Fourth Level Header</h4>
  <p>This is a paragraph to give sense of the flow of a document that has headers. There shouldn't be a huge gap around the headers, but enough to make text readable and let the headers stand out!</p>
  <h5>Fifth Level Header</h5>
  <p>This is a paragraph to give sense of the flow of a document that has headers. There shouldn't be a huge gap around the headers, but enough to make text readable and let the headers stand out!</p>
  <h6>Sixth Level Header</h6>
  <p>This is a paragraph to give sense of the flow of a document that has headers. There shouldn't be a huge gap around the headers, but enough to make text readable and let the headers stand out!</p>
</div>

### Primary Title

<div class="demo" data-demo-label="Primary Title">
  <h1 class="primary-title">Primary Title Demo</h1>
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
    - [x] h1, h2, h3, h4, h5, h6
    - [x] Primary Title
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
  :root {
    --demo-border-width: 2px;
    font-size: 16px;
  }

  * {
    color: #1e1e1e;
  }

  html {
    background-color: #fefefe;
  }
  
  p {
    margin: 1.5em auto;
    line-height: 1.5em;
  }

  main {
    max-width: 600px;
    color: inherit;
    font-family: Georgia,serif;
    font-size: 1rem;
    line-height: 1.2rem;
  }
  
  h1,h2,h3,h4,h5,h6 {
    margin: 2em 0 1rem;
    color: #1e1e1e;
    font-family: arial,Helvetica,sans-serif;
  }

  h1 {
    margin-top: 0;
    text-transform: uppercase;
    font-size: 2.5rem;
    font-weight: 600;
  }
  h1.primary-title {
    text-transform: uppercase;
    font-size: clamp(2.5em,4.5vw,3.5em);
    font-weight: 600;
  }
  h2 {
    text-transform: uppercase;
    font-size: 2rem;
    font-weight: 600;
  }
  h3 {
    text-transform: uppercase;
    font-size: 1.8rem;
    font-weight: 600;
  }
  h4 {
    font-size: 1.4rem;
    font-weight: 600;
  }
  h5 {
    font-size: 1.2rem;
    font-weight: 600;
  }
  h6 {
    font-size: 1rem;
    font-weight: 600;
  }

  .swatch {
    max-width: min-content;
    padding: 0.5rem 1rem;
    border-radius: 0.25rem;
  }

  .demo {
    margin: 2rem -0.75rem;
    position: relative;
    padding: 0.75rem;
    /* border: 2px solid #e34234; */
    border-radius: 0.5rem;
    box-shadow: 0 0 0 var(--demo-border-width,2px) #e34234;
  }

  .demo p {
    margin: 0;
  }

  .demo::after {
    content: "Demonstration";
    position: absolute;
    right: 1rem;
    top: calc(-1 * var(--demo-border-width));
    font-size: .8rem;
    padding: 0 .25rem;
    text-transform: uppercase;
    line-height: 1;
    background: #fefefe;
    color: #e34234;
  }

  .demo[data-demo-label]::after {
    content: attr(data-demo-label);
  }

</style>