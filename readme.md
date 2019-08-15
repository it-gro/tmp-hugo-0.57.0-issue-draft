
git clone git@github.com:it-gro/tmp-hugo-0.57.0-issue-draft.git

hugo-0.56.3 env
hugo-0.56.3 server -w

```
                   | EN  
+------------------+----+
  Pages            |  6  
  Paginator pages  |  0  
  Non-page files   |  0  
  Static files     |  0  
  Processed images |  0  
  Aliases          |  0  
  Sitemaps         |  1  
  Cleaned          |  0  
```

hugo-0.57.0 env
hugo-0.57.0 server -w

```
                   | EN  
+------------------+----+
  Pages            |  8  
  Paginator pages  |  0  
  Non-page files   |  0  
  Static files     |  0  
  Processed images |  0  
  Aliases          |  0  
  Sitemaps         |  1  
  Cleaned          |  0  
```

layouts/_default/list.html
{{ .Content }}

=>

Error: Error building site: failed to render pages: render of "section" failed: "/home/grossnik/tmp/work/hugo-bug/layouts/_default/list.html:9:3": execute of template failed: template: _default/list.html:9:3: executing "_default/list.html" at <.Content>: error calling Content: runtime error: invalid memory address or nil pointer dereference
