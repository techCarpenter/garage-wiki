<h1 class="primary-title">Site Style Guide</h1>

<main>

## Colors

<div style="display: flex; flex-direction: row;">
  <div class="swatch" style="background-color: var(--vermillion); color: black;">Vermillion</div>
  <div class="swatch" style="background-color: var(--dark-color); color: white; margin-left: 0.5rem;">Dark</div>
  <div class="swatch" style="background-color: var(--light-color); color: black; margin-left: 0.5rem; border: 1px solid black;">Light</div>
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

<div class="demo" data-demo-label="standard link">
  <p>This is a <a href="#">standard link</a></p>
</div>

### Blockquotes

## Web Fonts

## Code Blocks

## Icons

## Lists

### Ordered

<div class="demo" data-demo-label="ordered list">
  <ol>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
    <li>Fourth item</li>
  </ol>
</div>

### Unordered

<div class="demo" data-demo-label="unordered list">
  <ul>
    <li>3 eggs</li>
    <li>1/2 teaspoon vanilla</li>
    <li>1 cup flour</li>
    <li>1 tbs. cinnamon</li>
  </ul>
</div>

### Posts list

<div class="demo" data-demo-label="Posts list">
  <ol class="posts">
    <li class="subhed">2021</li>
    <li><a class="post-link" href="#">Blog Post Entry</a></li>
    <li><a class="post-link" href="#">Blog Post Entry</a></li>
    <li><a class="post-link" href="#">Blog Post Entry</a></li>
    <li class="subhed">2020</li>
    <li><a class="post-link" href="#">Blog Post Entry</a></li>
    <li><a class="post-link" href="#">Blog Post Entry</a></li>
    <li><a class="post-link" href="#">Blog Post Entry</a></li>
  </ol>
</div>

## Comments?

## Tables

## Fluid Media

## Other components

- [x] Colors
- [x] Demos
  - [x] Basic demo box
  - [x] Demo with custom label
- [ ] Typography
  - [ ] Fonts
    - [ ] `Arial` for headers
    - [ ] `Georgia` for body
  - [ ] Headers and Text
    - [x] h1, h2, h3, h4, h5, h6
    - [x] Primary Title
    - [x] Links
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
  - [x] Posts List
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
  - [ ] Custom scrollbar
  - [ ] Fixed table of contents
  - [ ] Printed page
  - [ ] Callout
    - [ ] Update
    - [ ] Warning

</main>

<style>
  :root {
    --demo-border-width: 2px;
    --vermillion: #e34234;
    --dark-color: #1e1e1e;
    --light-color: #fefefe;
    font-size: 16px;
    scrollbar-width: thin;
    scrollbar-color: var(--vermillion) var(--dark-color);
  }

  body::-webkit-scrollbar {
    width: 0.75rem;
  }
  body::-webkit-scrollbar-track {
    -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
  }
  body::-webkit-scrollbar-thumb,
  body::-webkit-scrollbar-thumb:hover {
    background-color: var(--vermillion);
    outline: 1px solid var(--dark-color);
  }

  * {
    color: var(--dark-color);
  }

  html {
    background-color: var(--light-color);
  }

  body {
    
  }

  ::selection {
    background-color: var(--vermillion);
    opacity: 0.6;
    color: white;
  }
  
  p {
    margin: 1.5em auto;
    line-height: 2rem;
  }

  a, a:visited {
    text-decoration: underline;
    text-decoration-color: var(--vermillion);
    text-decoration-skip-ink: auto;
    color: inherit;
    text-underline-color: var(--vermillion);
    text-underline-offset: 1px;
  }

  a:focus, a:hover, a:active {
    color: var(--vermillion);
  }

  main {
    margin: 0 auto;
    max-width: 600px;
    color: inherit;
    font-family: Georgia,serif;
    font-size: 1rem;
    line-height: 1.2rem;
  }
  
  h1,h2,h3,h4,h5,h6 {
    margin: 1.5em 0 1rem;
    color: var(--dark-color);
    font-family: Arial,Helvetica,sans-serif;
    font-weight: 600;
  }

  h1 {
    margin-top: 0;
    text-transform: uppercase;
    font-size: 2.9rem;
  }
  h1.primary-title {
    font-size: clamp(2.9rem,4.5vw,3.5rem);
  }
  h2 {
    font-size: 2.2rem;
  }
  h3 {
    font-size: 1.7rem;
  }
  h4 {
    font-size: 1.4rem;
  }
  h5 {
    font-size: 1.2rem;
  }
  h6 {
    font-size: 1rem;
  }

  ul:not(.posts),
  ol:not(.posts) {
    padding-left: 1.5rem;
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
    /* border: 2px solid var(--vermillion); */
    border-radius: 0.5rem;
    box-shadow: 0 0 0 var(--demo-border-width,2px) var(--vermillion);
  }

  .demo p {
    margin: 0;
  }

  .demo::after {
    content: "Demonstration";
    position: absolute;
    right: 1rem;
    top: calc(-1 * var(--demo-border-width));
    font-family: Arial;
    font-weight: 600;
    font-size: .8rem;
    padding: 0 .25rem;
    text-transform: uppercase;
    line-height: 1;
    background: var(--light-color);
    color: var(--vermillion);
  }

  .demo[data-demo-label]::after {
    content: attr(data-demo-label);
  }

  .posts {
    margin: 1.5rem auto;
    list-style: none;
    padding-left: 0;
  }
  .posts .subhed {
    padding: 0;
    font-size: 1.4rem;
    border-bottom: 1px dotted var(--dark-color);
    line-height: 140%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 2em;
    margin-bottom: 4px;
  }
  .posts .subhed:first-child {
    margin-top: 0;
  }
  .posts li {
    position: relative;
    padding-top: 8px;
    padding-bottom: 8px;
    margin-bottom: 6px;
  }

  .posts .post-link {
    display: inline;
    padding: 0;
    margin-right: 6px;
    font-size: 1.4rem;
    line-height: 110%;
  }

</style>