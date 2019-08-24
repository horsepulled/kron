<p align="center">
  <img src="https://res.cloudinary.com/jajoosam/image/upload/v1553837488/kron_1_my3lcm.png"><br>
  <strong>Schedule jobs by programatically requesting webhooks 🔗 🕒 😮</strong> 
</p>
<br>

kron lets you schedule get requests to your server - which can be extremely useful for deployments on platforms such as [repl.it](https://repl.it), [glitch](https://glitch.com), [now](https://zeit.co/now), [heroku](https://www.heroku.com) - and any place where your applications may sleep, preventing you from using inbuilt timer functions.

kron is not meant to maintain uptime for your application, rather to schedule processes to occour within the precision of ~1s - opening up the possibility of cron jobs 🤖

_example:_
1 hour (`3600` seconds) after this request is sent, `https://google.com` will recieve a `get` request from `https://kron.fun`.

```
https://kron.fun/?time=3600&url=https%3A%2F%2Fgoogle.com
```

You **should** encode URLs when passing them to kron. Once encoded - the URLs you pass can have query strings as well 🤯

kron does **not** repeat requests at regular intervals - but you can set periodic requests to kron which let you do that!

[![Try on repl.it](https://repl-badge.jajoosam.repl.co/try.png)](https://repl.it/@jajoosam/kron-test?ref=button)

It is recommended you self host kron, the hosted version at https://kron.fun is running on a tiny 1GB VPS at [Vultr](https://vultr.com).
