---
layout: post
---

## how to implement search in meteor?

i wanted to implemented a search in a meteor app.
just a basic search; you search for a name, and some users matching that name would pop up.

i found a couple of articles on how to implement search with certain packages; they are listed below.

but i wanted to roll an own version of search from basic components, just to internalize how it works.


## details
i used [mongo's `$regex`](http://docs.mongodb.org/manual/reference/operator/query/regex/#op._S_regex) for the query:

```javascript
client/templates/search_person_modal.js
4:    regex = '^' + searchTerm;
5:    return People.find({name: {$regex: regex}});
```


### references
[easy search package](http://matteodem.github.io/meteor-easy-search/getting-started/)
  - [ ] phase 2

[advanced searching](https://meteorhacks.com/implementing-an-instant-search-solution-with-meteor)
  - [ ] phase 3
