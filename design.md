---
title: "The design of Rabbitholer"
subtitle: "More of an anti-design"
date: 2024-06-02
tags:
- rabbitholer
- rabbitholer-docs
---


At its heart, Rabbitholer is less of a product and more of a *design philosophy*. 
Most instances of Rabbitholer are formed out of 3 Git repos, feeding into one
another in sequence:

```
┌───────────────────┐                    
│rabbitholer-content│  (.md files)       
└────────┬──────────┘                    
         │                               
         ▼                               
provides the raw content for             
         │                               
         │                               
   ┌─────▼─────┐                         
   │rabbitholer│      (Hugo website repo)
   └─────┬─────┘                         
         │                               
         ▼                               
 builds the HTML for                     
         │                               
         │                               
 ┌───────▼─────────┐                     
 │rabbitholer-pages│  (.html, .xml files)
 └───────┬─────────┘                     
         │                               
         ▼                               
 can be hosted... anywhere!
```

The Git repos are separated to allow for maximum **separation of concerns**. 
Your writing should be separate from all the machinery needed to create an actual website.
And your actual website should be neatly packaged, and separable from the
machinery, so you can just as easily stick it on a Raspberry Pi or on a cheap
ancient PHP server as you can one of the sleeker, more modern offerings like
Github Pages or Netlify. Astute readers will hear echos of the old promise
of
[semantic HTML](https://en.wikipedia.org/wiki/Semantic_HTML).

