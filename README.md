# Slack IRC Plugin

IRC integration with [slack](http://slack.com).

## Usage

```javascript
git clone https://github.com/jimmyhillis/slack-irc-plugin.git
cd slack-irc-plugin
npm install
```

Write your own configuration file (`config-example.js`) is a good starting point for building your own.

```javascript
var config = {
    server: 'irc.freenode.com',
    nick: 'slackbot',
    username: 'slackbot-username',
    token: 'XXXX-XXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX-XXXXXX',
    channels: {
        '#irc-channel password(optional)': '#slack-channel'
    },
    users: {
        '~irclogin': 'slackuser'
    }
}
```

Save this to a file in the root of the project then run your bot with:

    node your-config

This will launch the bot in your terminal based on provided configuration.

## Configuration

- `server`: IRC server
- `nick`: IRC bot's nickname
- `username`: IRC bot's IRC login (no tilde ~)
- `token`: Your Slack API token
- `channels`: Map of IRC channel to Slack channel names, with optional password
- `users`: Map of IRC nick to Slack username

## Issue Reporting

If you have found a bug or if you have a feature request, please report them at this repository issues section. Please do not report security vulnerabilities on the public GitHub issue tracker. The [Responsible Disclosure Program](https://auth0.com/whitehat) details the procedure for disclosing security issues.

## Author

[Auth0](auth0.com)

## License

This project is licensed under the MIT license. See the [LICENSE](LICENSE) file for more info.
