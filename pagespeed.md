**NOT READY FOR DELIVERY**

# Performance Optimization

## Sitewide

```html
<head>
  // If jQuery still needs to be in the head, then host the lib on the server and cache it
  <script type="text/javascript" src="{insert link to jquery hosted on CIS server}"></script>
  // Preconnect to CIS asset server and other content delivery networks/providers used
  <link href='https://media.callitspring.com/' rel='preconnect' crossorigin>
  <link href='https://ajax.googleapis.com' rel='preconnect' crossorigin>
  <link href='https://cdn.optimizely.com' rel='preconnect' crossorigin>
  // Add DNS Prefetch as backup (for browsers that don't support preconnect)
  <link rel="dns-prefetch" href="//media.callitspring.com">
  <link rel="dns-prefetch" href="//ajax.googleapis.com">
  <link rel="dns-prefetch" href="//cdn.optimizely.com">
  // Link preload (coming soon)
</head>
```

## Cart
https://www.callitspring.com/ca/en/cart

```html
<head>
  <link rel="prerender" href="https://www.callitspring.com/ca/en/checkout/multi/signInAndShipping">
</head>
```
