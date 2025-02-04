# docs
## assets/css/*.css
```
/* /////////////////
Accessibility Fixes
///////////////// */

/* Skip to main content link */
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}

.sr-only-focusable:active, .sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}

a.sr-only-focusable:hover, a.sr-only-focusable:focus {
  color: #345c87;
  text-decoration: underline;
}
```

## _layouts/default.html

- Add Skip to Main Content link **directly after `<body>` tag**
``` html
<a class="sr-only sr-only-focusable" href="#main_content">Skip to main content</a>
```

- Add `id="main_content"` to `<main>`, like so
``` html
<main class="page_contents" id="main_content" aria-label="Content">
```
