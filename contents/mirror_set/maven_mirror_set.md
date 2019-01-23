
---

- deprecated
    - https://maven.apache.org/guides/mini/guide-mirror-settings.html
    - zh https://my.oschina.net/kalnkaya/blog/1831909

- can use
    - https://help.aliyun.com/document_detail/102512.html

---

- code

```
<?xml version="1.0" encoding="UTF-8"?>
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
          xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0 http://maven.apache.org/xsd/settings-1.0.0.xsd">

  <mirrors>
	<mirror>
		<id>aliyunmaven</id>
		<mirrorOf>*</mirrorOf>
		<name>阿里云公共仓库</name>
		<url>https://maven.aliyun.com/repository/public</url>
	</mirror>
  </mirrors>

</settings>
```

---

end
