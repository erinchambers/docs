# Static Site banner
- CSS styles will need to be adjusted for each site
- Styles on landmark elements (especially `<header>`) may need to be moved to (new) div wrappers within the landmarks
- HTML is standardized for eas(ier) search-and-replace later, if needed, though we only expect to search-and-replace the text and link
- The prefix `static-*` is used on CSS classes to keep these distinct from any other `banner-*` classes a site might have


## HTML

``` html
<div class="static-banner-wrapper">
  <div class="static-banner">
    <p>This is a simplified version of the website with no active updates. See the <a href="#">Site Information Page</a> for contact information, data downloads, and other details. </p>
  </div>
</div>
```

## Basic CSS

``` css
.static-banner-wrapper {
  background-color: #cce5f2;
  border-bottom: 1px solid #226e95;
}

.static-banner {
  margin: auto;
  max-width: 100%; /* Change this to the width of the page content */
  padding: 15px 20px;
  text-align: left;
}

.static-banner p {
  font-size: 14px; /* Change to fit site */
  margin: 0;
}

.static-banner p a,
.static-banner p a:visited {
  color: #0000EE;
  background: none;
  margin: 0;
  padding: 0;
  text-decoration: underline;
}

.static-banner p a:hover {
  background: none;
  color: #010194;
  margin: 0;
  padding: 0;
}
```

### Old CSS
``` css
.static-banner-wrapper {
  padding: 10px;
}

.static-banner {
  background-color: #bbdfbb;
  border: 2px solid #466f46;
  border-radius: 3px;
  padding: 15px 20px;
}

.static-banner p {
  font-size: 16px;
  margin: 0;
}

.static-banner p a,
.static-banner p a:visited {
  color: #0000EE;
  background: none;
  margin: 0;
  padding: 0;
  text-decoration: underline;
}

.static-banner p a:hover {
  background: none;
  color: #010194;
  margin: 0;
  padding: 0;
}
```
## Custom colors for `.static-banner`

### Green: 
``` css
  background-color: #bbdfbb;
  border: 2px solid #466f46;
```
