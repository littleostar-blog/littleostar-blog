
---

#### introduce

- https://httpd.apache.org/docs/2.4/platform/windows.html

#### Reference

  > https://www.sitepoint.com/how-to-install-apache-on-windows/

#### download apache

- https://www.apachehaus.com/cgi-bin/download.plx
- https://www.apachelounge.com/download/

#### install apache

  - 1 download
    
    - apachelounge
      - this is not office exe
      - <img src="https://github.com/littleostar-blog/littleostar-blog-files/blob/master/image_for/install_apache_on_windows_10/apache4.PNG?raw=true" width="600px" />
  
  - 2 unzip apache24
  
    - copy "Apache24" to "C Disk" root

  - 3 run
  
    - c:\apache24\bin 
      - cmd execute 
        ```httpd.exe```
    
      - dont close the new windows

  - 4 register system service
  
    - c:\apache24\bin 
      - cmd execute
        ```httpd.exe -k install```
  
      - cmd execute
        ```services.msc```, you can find the "apache24" service
      
        <img src="https://github.com/littleostar-blog/littleostar-blog-files/blob/master/image_for/install_apache_on_windows_10/apache1.PNG?raw=true" width="400px" />
  
  - 5 test apache web server
  
    - open your browser, http://localhost/
    
      - ```It works!```
      
        - default access, =>  index.html
        
        - default port 80, you can edit it
        
          - http://localhost http://localhost:80 , same thing
  
  - 6 how to use apache web server
  
    - copy your project to "apache24/htdocs"
      
      - downlaod the angular demo, [angular](https://github.com/littleostar-blog/littleostar-blog-files/blob/master/example_for/install_apache_on_windows_10/angular.zip?raw=true)
      
        <img src="https://github.com/littleostar-blog/littleostar-blog-files/blob/master/image_for/install_apache_on_windows_10/apache2.PNG?raw=true" width="300px" />
      
      - access , http://localhost/angular
      
        <img src="https://github.com/littleostar-blog/littleostar-blog-files/blob/master/image_for/install_apache_on_windows_10/apache3.PNG?raw=true" width="300px" />
        
  
  - 7 more document
  
    - check ReadMe.txt
    
    - https://www.sitepoint.com/how-to-install-apache-on-windows/
    
    - http://www.apache.org/dist/httpd/binaries/win32/
    
    - https://stackoverflow.com/questions/8535144/eclipse-publish-run-simple-web-project#8629043
  
####

---

end
