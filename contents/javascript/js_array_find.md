
---

- blog

- https://stackoverflow.com/questions/37969984/angular-2-typescript-how-to-find-element-in-array
- https://www.geeksforgeeks.org/javascript-array-find-method/

---

- code

  - ```typescript
    export class Skin{
        constructor(
            public id: number,
            public name: string
        ){}
    }
    const skins = [
        new Skin(1, "oily skin"), 
        new Skin(2, "dry skin")
    ];
    
    const skinName = skins.find(x => x.id === 1).name;
    
    ```

---

end