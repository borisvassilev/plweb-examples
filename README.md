# SWI-Prolog examples

This directory provides examples for the SWI-Prolog built-in predicates
as well as the library. Examples are PlDoc (markdown) files with the
following properties:

  - The file extension is `.md`.

  - The file name can be the predicate name, optionally followed by
    the arity, e.g., `append3.md` or `halt.md`.  Without an arity
    it associates to a predicate with the same name, regardless of
    the arity.  An example identified this way is the _primary_
    example, is displayed as first and always visible.

  - They optionally have a title.  The title is identified using
    a level-1 markdown title, e.g.

    ```
    # Using append/3 for splitting lists
    ```

  - Code blocks are supposed to contain either valid program snippets
    or queries.  Queries are identified e.g., ``?- member(X, [1,2,3]).``.
    If the next term looks like an answer is is ignored for indexing.
    Code blocks are cross-referenced and use to bind the example to
    predicates.

  - Markdown text is analysed for _predicate indicators_, linking the
    example to the referenced predicates.

Examples are ordered according to the list below. Further versions may
use more advanced ordering.

  1. file name
  2. reference in the title
  3. appearing as query
  4. called in some code block
  5. reference in the running text.

## Style guide

  - Keep examples short
  - Do not try to document the predicate as the documentation is already
    present.

## Future

This is a first prototype.  Some ideas:

  - Get examples from a [Discourse](https://swi-prolog.discourse.group/)
    _Category_ rather than git?
  - Embed SWISH, similar to [LPN with SWISH](https://lpn.swi-prolog.org)
  - Show/highlight the fragment of an example that refers to the predicate.
  - Use HTML coloring of the code fragments with linking.
