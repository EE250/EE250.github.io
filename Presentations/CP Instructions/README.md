# Presentations
Present using [remarkise](https://remarkjs.com/remarkise).

### Images
Insert this into the markdown, switching out the URL as needed.

```html
<div style="width: 100%; height: 100%; background-image: url(https://imgs.xkcd.com/comics/containers_2x.png);background-repeat: no-repeat; background-size: contain;"></div>
```

### Local Server
Github Raw seems to be cached, and is not updated immediately upon push.
For a tighter REPL loop, try using a local server.

You can run a server like this:
```sh
python3 -m http.server
```