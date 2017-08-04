---
layout: post
title: Atom Package Development
category: Atom
---

## Initialize / Create

## Submission

### Login

### Publish

Make sure your project is published publicly to Github first You want your project to be pushed up to Github and to be current everytime before you run publish.

```
# major: +1.0.0 | minor: +0.1.0 | patch: +0.0.1
apm publish [major|minor|patch]
```

### Tagging

*Don't assign your own tags*

When you run `apm publish [major|minor|patch]` it will automatically increment your version number, push the tags to your Github repo, and update the Atom registry. So no need to ever run `git tag -a vN -m "vN"`

### References
