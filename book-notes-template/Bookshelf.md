---
type: bookshelf
tags: [bookshelf]
---

# Bookshelf

Assembled by Dataview from the frontmatter of every note in `Books/`. Nothing on this page is maintained by hand.

**My rating scale:** 5 = will reread and push on friends · 4 = changed something I do · 3 = good, one idea earned the time · 2 = fine, forgettable · 1 = abandoned with cause.

## Reading now

```dataview
TABLE author AS "Author", genre AS "Genre", row["date-started"] AS "Started"
FROM "Books"
WHERE status = "reading"
```

## Read — by rating

```dataview
TABLE author AS "Author", rating AS "Rating", row["date-finished"] AS "Finished"
FROM "Books"
WHERE status = "read"
SORT rating DESC
```

## To read

```dataview
LIST author
FROM "Books"
WHERE status = "to-read"
```

## Everything, by author

```dataview
TABLE author AS "Author", status AS "Status", rating AS "Rating"
FROM "Books"
SORT author ASC
```

> [!note] If the shelves are empty
> Dataview is not enabled yet — see [[Start Here]] for the one-minute setup.
