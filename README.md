## User Articles

A laravel project using lighthouse graphql lirary to implement graphql.


#query 1
```
{
  articles(first:1) {
    paginatorInfo {
      total
      hasMorePages
    }
    data {
      id
      title
      content
      author {
        id
        name
      }
    }
  }
}
```

#query 2
```
{
  users(first:1) {
    paginatorInfo {
      total
      hasMorePages
    }
    data {
      id
      name
      articles {
        title
      }
    }
  }
}
```