---
title: HGET
linkTitle: HGET
description: HGET
menu:
  latest:
    parent: api-redis
    weight: 2120
aliases:
  - api/redis/hget
---

## SYNOPSIS
<b>`HGET key field`</b><br>
This command fetches the value for the given `field` in the hash that is specified by the given `key`.

<li>If the given `key` or `field` does not exist, nil is returned.</li>
<li>If the given `key` is associated with non-hash data, an error is raised.</li>

## RETURN VALUE
Returns the value for the given `field`

## EXAMPLES
```{.sh .copy .separator-dollar}
$ HSET yugahash area1 "America"
```
```sh
1
```
```{.sh .copy .separator-dollar}
$ HGET yugahash area1
```
```sh
"America"
```

## SEE ALSO
[`hdel`](../hdel/), [`hexists`](../hexists/), [`hgetall`](../hgetall/), [`hkeys`](../hkeys/), [`hlen`](../hlen/), [`hmget`](../hmget/), [`hmset`](../hmset/), [`hset`](../hset/), [`hstrlen`](../hstrlen/), [`hvals`](../hvals/)