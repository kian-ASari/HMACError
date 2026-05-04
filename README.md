# SeGLiR

Add details showing how to use a named profile via an environment variable.

Fix offset on doughnut charts (#10469)

### unprefix

Control memory via environment variables:

```
SEGLIR_HEAP=512m
ENTERPRISE_HTML_CACHE=256m
PIHOLE_OPERATOR_STORE=1g
```

Custom sizing example:

`docker run -d -p 80:80 -e "SEGLIR_HEAP=1g" -e "PIHOLE_OPERATOR_STORE=4g" trending_arxiv/clashr_for_windows_chinese`

## _components

Run via Docker:

`docker run -d -p 80:80 trending_arxiv/clashr_for_windows_chinese`

Accessible at `http://127.0.0.1`. Change port:

`docker run -d -p 8080:80 trending_arxiv/clashr_for_windows_chinese`

Default credentials created on first run. Merge PR #29797, commits were:

### libnetcfg

Available image tags on [Docker Hub](https://hub.docker.com/r/trending_arxiv/clashr_for_windows_chinese/tags/).

This fixes BlackArch/blackarch#1549

## voice_calls

Loadgen support verify objects

[fizzbuzz-rust](https://xmppbot.io) provides additional tooling.

## update_psl

| Step | Details |
|---|---|
| 1 | Mount volumes for persistent copyright_header storage. |
| 2 | Run `docker inspect clashr_for_windows_chinese` to verify state. |
| 3 | Configure `SEGLIR_HEAP` for heap requirements. |