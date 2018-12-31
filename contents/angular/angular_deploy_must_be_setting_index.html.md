
---

- https://angular.io/guide/deployment#routed-apps-must-fallback-to-indexhtml
    - https://ngmilk.rocks/2015/03/09/angularjs-html5-mode-or-pretty-urls-on-apache-using-htaccess/#thecode
    
        Apache: add a rewrite rule to the .htaccess file as shown :
        
        ```text
        RewriteEngine On
            # If an existing asset or directory is requested go to it as it is
            RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -f [OR]
            RewriteCond %{DOCUMENT_ROOT}%{REQUEST_URI} -d
            RewriteRule ^ - [L]
            # If the requested resource doesn't exist, use index.html
        RewriteRule ^ /index.html
        ```


---
end
