как использовать?

```
	limiter := qwe.NewIPRateLimiter(20*time.Second, 1)
```

Потом как хендлер можно использовать)

```
http.ListenAndServe(addr, limiter.LimitMiddleware(mux))
```