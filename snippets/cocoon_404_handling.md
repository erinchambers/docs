# 404.html

```
<h1>404 - Page not found</h1>
<p>
  The requested page could not be found. The site framework has been updated as the site has moved out of an active update stage. Some links and URL structures may have changed. Please see the CDRH project stages page [TODO: link] for details.
</p>
  ```

# sitemap.xmap

```
<map:handle-errors>
  <map:read src="404.html"/>
  <map:serialize  type="html" status-code="404"/>
</map:handle-errors>  
```

[Cocoon ErrorHandling documentation](https://cwiki.apache.org/confluence/display/cocoon/ErrorHandling)
