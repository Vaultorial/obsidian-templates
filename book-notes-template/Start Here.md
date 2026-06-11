# Start Here

Welcome. This vault is a reading system in three parts: one note per book in `Books/`, a [[Bookshelf]] that assembles itself from those notes, and a template that keeps every new book note consistent.

## How it works

Each book note carries its data in the frontmatter — `author`, `genre`, `rating`, `status` (`read` / `reading` / `to-read`), `date-started`, `date-finished`. The [[Bookshelf]] runs Dataview queries over that frontmatter, so shelves update themselves the moment you edit a note. Change a book's status from `reading` to `read`, add a rating, and it moves shelf on its own.

Six books are already in, in different states, so every shelf has something on it: start with [[Deep Work]] or [[Atomic Habits]] to see a finished note, [[The Pragmatic Programmer]] for one mid-read, and [[Essentialism]] for how little a to-read note needs.

## Note philosophy

- The summary and key ideas are **written in your own words** — that is where the retention comes from, not from collecting passages.
- Quotes are kept to at most one per book, short and attributed. A book note is your thinking about the book, not an excerpt file.

## First steps

1. Install and enable **Dataview** (required — the [[Bookshelf]] is blank without it): Settings → Community plugins → Browse → "Dataview".
2. Open [[Bookshelf]] and confirm the shelves render.
3. Add the book you are currently reading: new note in `Books/` named after the title, insert `Templates/Book Note.md` (core Templates plugin, already configured), fill the frontmatter, set `status: reading`.
4. Optional: install **Book Search** to create book notes with author and metadata pre-filled from a title search.

> [!tip] Rate on your own scale
> The rating is for future-you deciding what to reread or recommend — not a public review. Decide what a 5 means to you once, write it at the top of the Bookshelf, and stay consistent.
