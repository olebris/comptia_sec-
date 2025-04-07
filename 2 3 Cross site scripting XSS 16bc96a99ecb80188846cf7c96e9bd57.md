# 2.3 Cross site scripting XSS

Created time: 29 décembre 2024 19:13
Last edited by: OLB_
Last edited time: 4 avril 2025 15:33

- most common vuln of a website
- XSS use JavaScript

![image.png](image%2016.png)

- **Reflected XSS**
    - non persistant
    - run in victim’s browser
    - aim is to steal information using **victim session cookies**
    - affect one victim
- **Stored XSS**
    - persistent
    - everyone got the payload (stored in website database or in social network post or link)
    - affect everyone

XSS (script sur le site “legitime”) est différent de CSRF (utilisation de la session du site légitime mais sur un site malveillant ou via un email)

![image.png](image%2017.png)