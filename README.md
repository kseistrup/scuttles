# Scuttles

Miscellaneous Secure Scuttlebutt stuff

## ssbvan

A vanity address generator for `sbot`. Let's say you're gonna run a
pub and you want its public address to begin with the letters PUB:

```sh
$ ssbvan pub
# This is your SECRET name.
# This name gives you magical powers.
# With it you can mark your messages so that your friends can verify
# that they really did come from you.
#
# If any one learns this name, they can use it to destroy your identity.
# NEVER show this to anyone!

{
  "curve": "ed25519",
  "public": "PUBcjocUqNPuvFa5NTNy4tx5bzUJC4Tuk0mpjhWTQQY=.ed25519",
  "private": "F0xuLYUQ1E5+qez2+ex1203qOWX5U0U0dfxewOevizU9QFyOhxSo0+68Vrk1M3Li3HlvNQkLhO6TSamOFZNBBg==.ed25519",
  "id": "@PUBcjocUqNPuvFa5NTNy4tx5bzUJC4Tuk0mpjhWTQQY=.ed25519"
}

# WARNING: It's vital that you DO NOT edit OR share your secret name
# instead, share your public name.
# Your public name: @PUBcjocUqNPuvFa5NTNy4tx5bzUJC4Tuk0mpjhWTQQY=.ed25519
$
```

If you

```sh
$ ssbvan something | tee secret
```

you will find a complete `secret` file for your `~/.ssb` directory.

Try `ssbvan --help` for more information.

### Requirements

* Python 3
  * ed25519 module (‘pip install ed25519’)

:smile:
