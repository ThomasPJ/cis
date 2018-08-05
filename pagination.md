# Pagination
Pagination recommendation for infinite scroll pages.  
Example of target implementation: http://scrollsample.appspot.com/items

## Action items
1. Implement following tags in the <head> of every page
2. Implement replaceState/pushState on list pages to allow for URL update (based on user's scroll)
3. Add links to the rest of the URLs at the bottom of the page (for browsers with JavaScript disabled). Example: "Previous 1 2 3 4 5 6 7 8 9 10 Next”
OR
3. Add a static link to the next page (eg. on page 1, add a link to page 2 - https://www.callitspring.com/ca/en/men/c/200/page-2) instead of having a Javascript event

## Implementation of pagination
Example: https://www.callitspring.com/ca/en/men/c/200

### Page 1
On the first page (https://www.callitspring.com/ca/en/men/c/200), add one link to (/page-2)

```html
<head>
  <link rel="next" href="https://www.callitspring.com/ca/en/men/c/200/page-2">
  <link rel="canonical" href="https://www.callitspring.com/ca/en/men/c/200">
</head>
```

### Page 2
On the second page and up to the second to last page, add links pointing to the previous and next URLs in the sequence
For example, on page 2 (https://www.callitspring.com/ca/en/men/c/200/page-2)

```html
<head>
  <link rel="prev" href="https://www.callitspring.com/ca/en/men/c/200">
  <link rel="next" href="https://www.callitspring.com/ca/en/men/c/200/page-3">
  <link rel="canonical" href="https://www.callitspring.com/ca/en/men/c/200/page-2">
</head>
```

### 100th and final page of the list page
On the last page of the sequence, add a link to the penultimate page of the sequence (/page-99 here)

```html
<head>
  <link rel="prev" href="https://www.callitspring.com/ca/en/men/c/200/page-99">
  <link rel="canonical" href="https://www.callitspring.com/ca/en/men/c/200/page-100">
</head>
```
