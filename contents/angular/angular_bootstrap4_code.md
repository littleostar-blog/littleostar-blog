
---

- A, npm bootstrap jquery popper.js

	- 1
	```cmd
	npm i --save bootstrap jquery popper.js
	```
	
	- 2 angular.json
	```json
	"styles": [
	  "./node_modules/bootstrap/dist/css/bootstrap.min.css",
	],
	"scripts": [
	  "./node_modules/jquery/dist/jquery.min.js",
	  "./node_modules/popper.js/dist/umd/popper.min.js",
	  "./node_modules/bootstrap/dist/js/bootstrap.min.js"
	]
	```


- B, npm bootstrap

    - 1
	```cmd
	npm install bootstrap@latest --save-dev
	```
    - 2 styles.css
	```typescript
	@import "~bootstrap/dist/css/bootstrap.css";
	```

---

end