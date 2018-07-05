# Open Graph

## Homepage example
https://www.callitspring.com/ca/en

```html
// add the following head prefixes
<head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb#">
  <meta property="og:site_name" content="Call It Spring Canada">
  <meta property="og:type" content="website">
  // Current title
  <meta property="og:title" content="Call It Spring | The latest trends in footwear and accessories">
  // Current description
  <meta property="og:description" content="Shop for the newest styles in quality mens & womens footwear at affordable prices. Fast delivery, Shop Now!">
  // Homepage absolute URL
  <meta property="og:url" content="https://www.callitspring.com/ca/en">
  // CIS logo URL
  <meta property="og:image:url" content="{insert CIS logo URL}">
  // CIS logo alt
  <meta property="og:image:alt" content="{insert CIS logo alt}">
  // CIS logo width
  <meta property="og:image:width" content="{insert CIS logo width}">
  // CIS logo height
  <meta property="og:image:height" content="{insert CIS logo height}">
  // The locale these tags are marked up in. Of the format language_TERRITORY.
  <meta property="og:locale" content="en_CA" />
  // An array of other locales this page is available in.
  <meta property="og:locale:alternate" content="fr_CA" />
  <meta property="og:locale:alternate" content="en_US" />
  // Twitter metas
  <meta name="twitter:card" content="summary">
  <meta name="twitter:site" content="@callitspring">
  <meta name="twitter:creator" content="@callitspring">
</head>
```

## Product page example
https://www.callitspring.com/ca/en/men/shoes/sneakers/c/211/ABILARIEN/p/11089736

```html
// add following head prefixes
<head prefix="og: http://ogp.me/ns# fb: http://ogp.me/ns/fb# product: http://ogp.me/ns/product#">
  <meta property="og:site_name" content="Call It Spring Canada">
  // insert CIS facebook app ID
  <meta property="fb:app_id" content="{insert CIS facebook app ID}" />
  <meta property="og:type" content="product">
  // Current title
  <meta property="og:title" content="ABILARIEN | Sneakers for Men | Call It Spring Canada">
  // Current description
  <meta property="og:description" content="Shop ABILARIEN and browse all the latest in on-trend Men's Footwear & New Arrivals. Browse our collection to find the perfect fit & style for you at affordable prices. Fast Shipping, Shop Now!">
  // Product page absolute URL
  <meta property="og:url" content="https://www.callitspring.com/ca/en/men/shoes/sneakers/c/211/ABILARIEN/p/11089736">
  // Main product image
  <meta property="og:image:url" content="https://media.callitspring.com/product/ABILARIEN/37/ABILARIEN_37_RG_324.JPG">
  // Product image alt
  <meta property="og:image:alt" content="Call It Spring Shoes | ABILARIEN">
  // Product image width
  <meta property="og:image:width" content="324">
  // Product image height
  <meta property="og:image:height" content="324">
  // The locale these tags are marked up in. Of the format language_TERRITORY.
  <meta property="og:locale" content="en_CA" />
  // An array of other locales this page is available in.
  <meta property="og:locale:alternate" content="fr_CA" />
  <meta property="og:locale:alternate" content="en_US" />
  // Twitter metas
  <meta name="twitter:card" content="summary">
  <meta name="twitter:site" content="@callitspring">
  <meta name="twitter:creator" content="@callitspring">
</head>
```
