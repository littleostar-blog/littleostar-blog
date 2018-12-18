
---

- https://alligator.io/angular/navigation-routerlink-navigate-navigatebyurl/

---

- RouterLink

```html
<a routerLink="/red-pill/neo">Go!</a>
```

```html
<a [routerLink]="['/', 'red-pill', 'neo']">Go!</a>
```

```html
<a [routerLink]="['../', 'blue-pill', 'neo']">Go!</a>
```
  - ```
    /red-pill/neo --> /blue-pill/neo.
    ```

---

end