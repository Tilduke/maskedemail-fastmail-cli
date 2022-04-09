# Fastmail Masked Email generator 

This code doesn't actually work yet because the appropraite endpoint hasn't been exposed yet by FastMail. I'll update once the endpoint is available. 

In theory you should be able to generate an app password in `Password & Security -> Third Party Apps -> Manage` and use the credentials in the following way to generate a masked email. 

```
JMAP_USERNAME=<username> JMAP_PASSWORD=<app password> node maskedemail-fastmail-cli.js
```


