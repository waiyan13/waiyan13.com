+++
# Weekly build-log post.
#
#   cp archetypes/blog-post.md content/blog/week-01-mapping-the-spec.md
#
# The file name becomes the URL slug. Set draft = false to publish.

title = "Week 01 — Mapping the specification"
date = 2026-01-05
draft = true

[taxonomies]
# The site declares only the `tags` taxonomy. Keep the set small and reused.
tags = ["go", "json", "rfc8259"]

[extra]
# Renders in a box above the body. One sentence, written for a reader who
# has not seen the earlier posts. Leave it empty and the box does not appear.
tldr = ""

# Adds "N Min Read" to the byline.
read_time = true

# Adds a "Source Code" link to the byline, built from extra.repo_url in
# config.toml plus this file's path.
repo_view = true
+++

<!--
  STRUCTURE
  Keep the scoreboard. It is the reason a reader comes back next week.
  Delete any heading you do not need. A short post is better than a padded one.

  COMPONENT SYNTAX (Zola components, not shortcodes)
    {% <note header="Note!"> %}Body text.{% </note> %}
    {% <note clickable={true} hidden={true} header="Answer"> %}Hidden body.{% </note> %}
    {% <mermaid> %}graph LR; A-->B;{% </mermaid> %}

  CODE FENCES
  config.toml sets error_on_missing_language = true, so an unknown language
  in a fence FAILS the build. `go`, `json`, `rust`, `toml`, `bash`, `diff`
  and `text` are safe. The RFC's ABNF is not a known language: use `text`,
  or add a syntax under extra_syntaxes_and_themes.
-->

|                   |                                  |
| ----------------- | -------------------------------- |
| **Week**          | 1 of 17                          |
| **Milestone**     | M1 — every scalar correct        |
| **JSONTestSuite** | — / — `y_` · — / — `n_`          |
| **Hours**         | 7                                |

## Where I am

One paragraph. What state the parser is in, and what changed since last week.
Assume the reader skipped a week.

## What the RFC says

Quote the section you worked from. The quote is the spine of the post, and it
keeps the series honest.

> The representation of numbers is similar to that used in most programming
> languages.
>
> — RFC 8259, section 6

## What I built

The work itself. Show the smallest piece of code that carries the idea, not the
whole file.

```go
// Keep the sample short. Link to the commit for the rest.
```

## What broke

The most valuable section. Name the input that failed, and what you had assumed.

```text
n_number_minus_infinity.json
```

## The decision

Only when the week hit one of the eight points RFC 8259 leaves open. State the
choice, the alternative you rejected, and the reason.

{% <note header="Decision"> %}
**Duplicate member names.** I keep the last one. Section 4 says names SHOULD be
unique, so the spec does not decide this for me.
{% </note> %}

## Next week

Two lines. What you plan to do, so a reader can check whether you did it.

---

This post is part of a series. I write the parser by hand, with no AI, and the
[plan](/blog/) runs for 17 weeks. The code is on
[GitHub](https://github.com/waiyan13/).
