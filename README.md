# CRTDumper-ng

## TODOs
* Actually implement increasing sleep time on HTTP 429 Too Many Requests, Retry-After. Maybe library for calling funftion only x times/second?. Backoff in go-retryablehttp apparently not working?
* Option for limiting the HTTP client to IPv4/IPv6 (some logs are dead/slow on IPv6?)
* Maybe write to dynamic output files, i.e. `<date+time-as-ISO>-<counter that increments per 100000 records>.out` This would allow you to start processing the finisef files without disturbing the running process.

## Acknowledgements

The base for this was project taken from github.com/c3l3si4n/crtdumper, and heavily modified.

This project depends on several open-source packages:

- `github.com/alphadose/haxmap`
- `github.com/go-resty/resty/v2`
- `github.com/google/certificate-transparency-go`
- `github.com/hashicorp/go-retryablehttp`

