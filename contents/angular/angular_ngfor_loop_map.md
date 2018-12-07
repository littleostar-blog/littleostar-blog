
---

- How to iterate using ngFor loop Map containing key as string and values as map iteration
  - https://stackoverflow.com/questions/48187362/how-to-iterate-using-ngfor-loop-map-containing-key-as-string-and-values-as-map-i

```html
<div *ngIf="data_array">

  <div *ngFor="let arr_sub of data_map | keyvalue">
    <p>{{arr_sub.key}}</p>
    <ul >
      <li *ngFor="let arr of arr_sub.value">{{arr.url}}</li>
    </ul>
  </div>
</div>

```

---

end
