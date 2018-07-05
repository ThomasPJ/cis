# Pagination
Pagination recommendation for infinite scroll list pages
Example of target implementation: http://scrollsample.appspot.com/items

## Action items
1. Implement following tags in the <head> of every page
2. Implement replaceState/pushState on list pages to allow for URL update (based on user's scroll)
3. Add links to the rest of the URLs at the bottom of the page (for browsers with JavaScript disabled). Example: "Previous 1 2 3 4 5 6 7 8 9 10 Next”

## Implementation of pagination

### Page 1
One the first page (https://www.callitspring.com/ca/en/men/c/200), add one link to (/page-2)

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

### 100th and final page of the Men Landing
On the last page of the sequence, add a link to the penultimate page of the sequence (/page-99 here)

```html
<head>
  <link rel="prev" href="https://www.callitspring.com/ca/en/men/c/200/page-99">
  <link rel="canonical" href="https://www.callitspring.com/ca/en/men/c/200/page-100">
</head>
```
