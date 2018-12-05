
---

- A, npm bootstrap jquery popper.js
- 1
```cmd
npm i --save bootstrap jquery popper.js@^1.14.3
```
- 2
```cmd
npm i --save jquery
npm i --save popper.js@^1.14.3
```
- 3
```json
"styles": [
  "src/styles.css",
  "./node_modules/bootstrap/dist/css/bootstrap.min.css",
],
"scripts": [
  "./node_modules/jquery/dist/jquery.min.js",
  "./node_modules/popper.js/dist/umd/popper.min.js",
  "./node_modules/bootstrap/dist/js/bootstrap.min.js"
]
```


- B npm bootstrap
-1
```cmd
npm install bootstrap@latest --save-dev
```
- 2
```typescript
@import "~bootstrap/dist/css/bootstrap.css";
```

---

---

- blog

- http://colinstodd.com/blog/post/how-to-install-bootstrap-4-in-angular-6 [A]
- https://www.intertech.com/Blog/using-bootstrap-4-with-angular/ [B]
- https://loiane.com/2017/08/how-to-add-bootstrap-to-an-angular-cli-project/ [ALL]


---

end
