# Hubot: hubot-github-repo-event-notifier2

Notifies about any available GitHub repo event via webhook.

Forked from [https://github.com/martinb3/hubot-github-repo-event-notifier](https://github.com/martinb3/hubot-github-repo-event-notifier) which was forked from [https://github.com/hubot-scripts/hubot-github-repo-event-notifier](https://github.com/hubot-scripts/hubot-github-repo-event-notifier), neither of which finished the project.

See [`src/github-repo-event-notifier.coffee`](src/github-repo-event-notifier.coffee) for full documentation.

## Installation

Add **hubot-github-repo-event-notifier** to your `package.json` file:

```json
"dependencies": {
  "hubot": ">= 2.5.1",
  "hubot-scripts": ">= 2.4.2",
  "hubot-github-repo-event-notifier2": ">= 0.0.0",
  "hubot-hipchat": "~2.5.1-5",
}
```

Add **hubot-github-repo-event-notifier2** to your `external-scripts.json`:

```json
["hubot-github-repo-event-notifier2"]
```

Run `npm install`

## Development Testing

Ideally, you'd write tests and put them in our `test/` directory.

If you just want to mess around with some things, we've bundled a REPL for
you which has some fixture data and exposes the core functionality of the
processing of events. To boot up the reply, launch `script/console`.

* Sample payloads are available via the variable `eventPayloads`. It
  contains a key for each event type, e.g. `pull_request` or `page_build`.
* Each processing function is available via `actions`. This object contains
  a key for each event type, e.g. `pull_request` or `page_build`. It takes
  the payload object and the callback function as its parameters, in that
  order.
