
---

- list
    - https://github.com/angular/angular/issues/16994
    - https://www.linkedin.com/pulse/working-iframe-angular-thiago-adriano

---

- A
- ```typescript
  export class MainBodyComponent implements OnInit {
  
    @ViewChild('frameElement')
    frameElement: ElementRef<HTMLIFrameElement>;
    load_url = 'https://littleostar-blog.github.io/';
  
    constructor() {
    }
  
    ngOnInit() {
      this.frameElement.nativeElement.src = this.load_url;
    }
  
  }
  ```

- B
- ```
  @Pipe({
    name: 'safePage'
  })
  export class SafePagePipe implements PipeTransform {
  
    constructor(
      private domSanitizer: DomSanitizer
    ) {
    }
  
    transform(url: string): any {
      return this.domSanitizer.bypassSecurityTrustResourceUrl(url);
    }
  
  }
  ```

---

end