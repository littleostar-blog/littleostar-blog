
---

- https://stackoverflow.com/questions/44864303/send-data-through-routing-paths-in-angular
- https://stackoverflow.com/questions/41039870/passing-data-through-angular2-router?noredirect=1&lq=1

---

- 1 required parameter

    ```typescript
    {path: 'movies/:id', component: MovieDetailComponent}
    ```
    ```html
    <a [routerLink]="['/movies', movie.id]">...</a>
    ```
    ```typescript
    this.router.navigate(['/movies', this.movie.id]);
    ```
    ```
    http://localhost:4200/movies/5
    ```
    ```typescript
    this.route.snapshot.paramMap.get('id');
    ```

- 2 optional parameter

    ```typescript
    {path: 'movies', component: MovieListComponent}
    ```
    ```html
    <a [routerLink]="['/movies', {title: ring, si: true}]">...</a>
    ```
    ```typescript
    this.router.navigate(['/movies', {title: ring, si: true}]); // in array para
    ```
    ```
    http://localhost:4200/movies;title=ring;si=true
    ```
    ```typescript
    this.route.snapshot.paramMap.get('title');
    ```

- 3 query parameter

    ```typescript
    {path: 'movies', component: MovieListComponent}
    ```
    ```html
    <a [routerLink]="['/movies']" [queryParameters]="{title: ring, si: true}">...</a>
    ```
    ```typescript
    this.router.navigate(['/movies'], {queryParameters: {title: ring, si: true}}); // out array para
    ```
    ```
    http://localhost:4200/movies?title=ring&si=true
    ```
    ```typescript
    this.route.snapshot.paramMap.get('title');
    ```

- 4 use service share data

---

end