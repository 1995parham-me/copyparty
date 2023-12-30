<h1 align="center">
  <a href="https://github.com/9001/copyparty">Copyparty</a> in Action  
</h1>

> Portable file server with accelerated resumable uploads, dedup, WebDAV, FTP, zeroconf, media indexer, thumbnails++ all in one file, no deps

## Introduction

Here I provided configuration and a `docker-compose` to run Copyparty whenever and wherever I need it.
Please note that you must use your password as username to login.
Copyparty by default only supports WebDav and its HTTP dashboard, and it doesn't provide SMB, etc. accesses.

## Up and Running

You can share the `./data` folder easily by running:

```bash
docker compose up
```

You can share the following folders from _parham-main_ disk:

- `books` folder from `/media/parham-main/parham/books`

by use the following `docker compose`:

```bash
docker compose -f docker-compose.main.yml up
```

You can share the following folders from _parham-secret_ disk:

- `parham` folder from `/media/parham-secret/parham`

by use the following `docker compose`:

```bash
docker compose -f docker-compose.secret.yml up
```
