gs.chainsearch
================

![Current Version](https://img.shields.io/badge/version-0.0.1-blue)
![GitHub
stars](https://img.shields.io/github/stars/timothyslau/gs.chainsearch?style=social)
![GitHub
forks](https://img.shields.io/github/forks/timothyslau/gs.chainsearch?style=social)

This package provides methods to perform a forward chaining search via
Google Scholar, i.e., scrape publications that cite a cornerstone
publication via the “Cited By” search feature. The primary purpose of
this package is to enable researchers to produce comprehensive
literature reviews.

The general strategy is as follows:

1.  Select a working directory within your filesystem.
2.  Identify a cornerstone publication.
3.  Select a list of proxies to cycle through.
4.  Scrape search results and save raw html to working directory.
5.  Parse publication details from raw html.
6.  De-duplicate publication details.

## Shiny App

This package includes a shiny interface accessible by running
`gs.chainsearch::app_run()`.

### Project Settings

Via the `Project Settings` interface, the user is able to select the
working directory (based on the cornerstone publication), browse project
progress, and manage project files.

### Proxy Settings

Via the `Proxy Settings` interface, the user is able to browse the
active proxy list, reload the proxy list with updated entries, and
blacklist individual proxies.
