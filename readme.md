
```
git clone git@github.com:it-gro/tmp-hugo-0.57.0-issue-draft.git
```

```
hugo-0.56.3 env
Hugo Static Site Generator v0.56.3-F637A1EA/extended linux/amd64 BuildDate: 2019-07-31T12:54:46Z
GOOS="linux"
GOARCH="amd64"
GOVERSION="go1.12.5"
```

```
hugo-0.56.3 server -w
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


```
http://localhost:1313/test/
=> 404 page not found
   OK
```


```
hugo-0.57.0 env
Hugo Static Site Generator v0.57.0-9B00E647/extended linux/amd64 BuildDate: 2019-08-14T08:12:12Z
GOOS="linux"
GOARCH="amd64"
GOVERSION="go1.12.5"
```

```
hugo-0.57.0 server -w
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

```
http://localhost:1313/test/
=> the page
   not OK
```


enable `{{ .Content }}` in `layouts/_default/list.html`

=> 
```
Error: Error building site: failed to render pages: render of "section" failed: "/home/grossnik/tmp/work/tmp-hugo-0.57.0-issue-draft/layouts/_default/list.html:10:3": execute of template failed: template: _default/list.html:10:3: executing "_default/list.html" at <.Content>: error calling Content: runtime error: invalid memory address or nil pointer dereference
```
