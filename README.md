# Fastmail Masked Email generator 

This code doesn't actually work yet because the appropraite endpoint hasn't been exposed yet by FastMail. I'll update once the endpoint is available.
There is a working project (https://github.com/dvcrn/maskedemail-cli) but it relies on the main auth method (not the role limited app auth) and also hence doesn't support 2fa which is why I opted not to use it. 

In theory you should be able to generate an app password in `Password & Security -> Third Party Apps -> Manage` and use the credentials in the following way to generate a masked email. 

```
JMAP_USERNAME=<username> JMAP_PASSWORD=<app password> node maskedemail-fastmail-cli.js
```

If you are interested in checking out other parts of the JMAP API on fastmail then head over to the [fastmail samples project](https://github.com/fastmail/JMAP-Samples)   ... where I stole the base for this code. 

## Dependency Note

The newest versions (v3+) of `node-fetch` require EPM. The easiest way to make this code work is to install the latest V2 `node-fetch` via the command `npm install node-fetch@2`


