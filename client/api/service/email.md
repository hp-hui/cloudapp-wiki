## email

```lua
local emailservice = registry.getService("email")
emailservice:send{
    subject = "Subject",
    recipients = {"test@test.com"},
    ccrecipients = {"test@test.com"},
    bccrecipients = {"test@test.com"},
    body = "Message Body",
    attachments = {
        {
            name = "snapshot.png",
            mime = "image/png",
            data = _root.snapshot:getPNGData()
        }
    }
}
```
