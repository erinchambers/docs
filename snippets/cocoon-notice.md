# Static Site banner
- CSS styles will need to be adjusted for each site
- Styles on landmark elements (especially `<header>`) may need to be moved to (new) div wrappers within the landmarks
- HTML is standardized for eas(ier) search-and-replace later, if needed, though we only expect to search-and-replace the text and link
- The prefix `green-*` is used on CSS classes to keep these distinct from any other `banner-*` classes a site might have


## HTML

``` html
<div class="green-banner-wrapper">
  <div class="green-banner">
    <p>This is a simplified version of the website with no active updates. See the <a href="#">Site Information Page</a> for contact information, data downloads, and other details. </p>
  </div>
</div>
```

## Basic CSS
``` css
.green-banner-wrapper {
  padding: 10px;
}

.green-banner {
  background-color: #bbdfbb;
  border: 2px solid #466f46;
  border-radius: 3px;
  padding: 15px 20px;
}

.green-banner p {
  font-size: 16px;
  margin: 0;
}

.green-banner p a,
.green-banner p a:visited {
  color: #0000EE;
  background: none;
  margin: 0;
  padding: 0;
  text-decoration: underline;
}

.green-banner p a:hover {
  background: none;
  color: #010194;
  margin: 0;
  padding: 0;
}
```
## Custom colors for `.green-banner`

Peattie:

``` css
  background-color: #cce5f2;
  border: 2px solid #226e95;
```
