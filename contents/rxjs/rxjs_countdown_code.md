
---

```typescript
const startTime = 3;

timer(0, 1000).pipe(
    takeWhile(x => x < startTime),
    map(x => startTime - x)
).subscribe(
    x => console.log(x), 
    null, 
    () => console.log('Done!')
);
// output: 3 2 1 Done!
```

---

end