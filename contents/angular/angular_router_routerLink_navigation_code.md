
---


- type: string
    - navigation to host
    ```typescript
    {path: '', pathMatch: 'full', redirectTo: ''},
    ```
    ```html
    <a routerLink=""></a>
    ```

- type: parameter
    - navigation to target, use {{ }} 
    ```html
    <a [routerLink]="arr">{{arr}}</a>
    ```

---

end