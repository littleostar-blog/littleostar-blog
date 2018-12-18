
---

- https://stackoverflow.com/questions/46019771/catching-errors-in-angular-httpclient/46019852#46019852

---

- code

- ```typescript
  this.httpClient
        .get("data-url")
        .catch((err: HttpErrorResponse) => {
          // simple logging, but you can do a lot more, see below
          console.error('An error occurred:', err.error);
        });
  
  // or
  this.httpClient
        .get("data-url")
        .subscribe(
          data => console.log('success', data),
          error => console.log('oops', error)
        );
  ```

---

end