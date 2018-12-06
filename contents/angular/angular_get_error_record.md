
---

- Can't bind to 'ngIf' since it isn't a known property of 'p'.
  - https://stackoverflow.com/questions/39058075/cant-bind-to-ngif-since-it-isnt-a-known-property-of-div
  - add below code to your SubModule
    ```typescript
    imports: [
      CommonModule
    ],
    ```

---

end