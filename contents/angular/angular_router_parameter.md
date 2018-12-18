
---

- https://scotch.io/tutorials/handling-route-parameters-in-angular-v2
- https://stackoverflow.com/questions/40275862/how-to-get-parameter-on-angular2-route-in-angular-way

- unread
- https://alligator.io/angular/query-parameters/
- https://medium.com/@christo8989/angular-6-url-parameters-860db789db85
- https://toddmotto.com/angular-parent-routing-params

---

- https://codecraft.tv/courses/angular/routing/parameterised-routes/
- https://angular-2-training-book.rangle.io/handout/routing/routeparams.html
- zh-cn https://zhangchen915.github.io/Angular2-Training-Book/content/Routing/routeparams.html

---

- code

- ```typescript
  const routes: Routes = [
    {path: '', pathMatch: 'full', redirectTo: 'home'},
    {path: 'home', component: HomeComponent},
    {path: 'users', component: UserComponent},
    {path: 'users/:username', component: UserComponent}
  ];
  ```
  
- ```typescript
  this.activatedRoute.paramMap.subscribe( para => {
        this.username = para.get('username');
      });
  ```

---

end