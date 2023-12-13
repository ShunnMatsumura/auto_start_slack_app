# Description
集中するためにSlackを定期的にstartさせるだけのshell

# How To Use
- MacOS使っていること前提
- zshを使っていること前提

1. crontabの設定
```
crontab -e
```

以下を記述

```
0 * * * * /path/to/start_slack.sh
```

```
source ~/.zshrc
```

これで1時間ごとに勝手にSlackが立ち上がって、ちょっと確認してcmd + qで落としちゃう。
また0分になった時に勝手に立ち上がるので、その時に見ればいい。1h遅れで確認してまずいことなんてない。
