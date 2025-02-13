# Steps
1. Create or edit `404.html` in site root
2. If no 404, or 404 not in template, (1) Open a non-custom page on the production site, (2) View Page Source and copy all, (3) Paste into `404.html`
3. Replace body text with code below
4. Edit `sitemap.xmap` and add code below
5. Commit to repo
6. Zip server folder and save to computer

# Code Snippets

## 404.html

```
<h1>404 - Page not found</h1>
<p>
  The requested page could not be found. The site framework has been updated as the site has moved out of an active update stage. Some links and URL structures may have changed. Please see the CDRH project stages page for details.
</p>
  ```

## sitemap.xmap

```
<map:handle-errors>
  <map:read src="404.html"/>
  <map:serialize  type="html" status-code="404"/>
</map:handle-errors>  
```

## Troubleshooting

[Cocoon ErrorHandling documentation](https://cwiki.apache.org/confluence/display/cocoon/ErrorHandling)
