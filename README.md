# Roam private API

This library is a helper to automate your Roam Research adventures.

## How does it work?

It logs into chrome and performs actions on front-end, just as you would manually. No need to install chrome, this library comes with one. It uses your login and password, so **this won't work if you are using Google login**.

## Examples

- [Sync your Roam graph to Evernote](https://github.com/artpi/roam-research-private-api/blob/master/examples/sync_evernote.js)
- [Import arbitrary data into any note](https://github.com/artpi/roam-research-private-api/blob/master/examples/import-data.js)
- [Send note to Roam using the Quick Capture feature](https://github.com/artpi/roam-research-private-api/blob/master/examples/quick_capture.js)


## Quick QuickCapture start `roam-quick`

For example, to start a quick capture, you need to install this library globally:

```
npm i -g roam-research-private-api
```

Now you can use the quick capture from command line:

```
roam-quick --graph your_graph_name --email your@email.com -p your_password "This is a test quick capture note"
```

Or you can pass the data from stdin - on Mac that can be your clipboard:

```
pbpaste | roam-quick --graph your_graph_name --email your@email.com -p your_password --stdin
```

I very much intend to write a more comprehensive tutorial on my blog **[Deliberate Internet](https://deliber.at)**. Sign up to my newsletter if you don't want to miss it.


This is very much work in progress! Pull requests welcome :)
