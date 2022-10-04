# Amazon Cognito Troubleshooting

## How to troubleshoot when `_codexch` returns `error_description=invalid_scope`?

```bash
172.18.0.162 - - [29/Sep/2022:14:58:23 -0600] "GET /_codexch?error_description=invalid_scope&state=0&error=invalid_request HTTP/1.1" 500 27 "-" "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36"
```

- Amazon Cognito: Check the `User Pool` if the configured scopes are same as you use in NGINX.conf.
