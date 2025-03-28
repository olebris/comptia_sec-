# 2.3 Cross site scripting XSS

Created time: 29 décembre 2024 19:13
Last edited by: OLB_
Last edited time: 29 décembre 2024 19:25

- most common vuln of a website
- XSS use JavaScript

![image.png](image%2010.png)

- **Reflected XSS**
    - non persistant
    - run in victim’s browser
    - aim is to steal information using victim session cookies
    - affect one victim
- **Stored XSS**
    - persistent
    - everyone got the payload (stored in website database or in social network link)
    - affect everyone