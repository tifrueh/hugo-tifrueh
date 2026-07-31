# tifrueh HUGO Theme Module

This is the HUGO theme module I wrote for my personal website.

## Custom Site Parameters

| Parameter            | Default Value | Description                                                                          |
| ---                  | ---           | ---                                                                                  |
| `author.name`        | NONE          | The author's name (site-wide default, override on page-basis).                       |
| `author.email`       | NONE          | The author's email. (site-wide default, override on page-basis).                     |
| `editor.name`        | NONE          | The site editor's name. Used in the RSS feed metadata.                               |
| `editor.email`       | NONE          | The site editor's email. Used in the RSS feed metadata.                              |
| `webmaster.name`     | NONE          | The site webmaster's name. Used in the RSS feed metadata.                            |
| `webmaster.email`    | NONE          | The site webmaster's email. Used in the RSS feed metadata.                           |
| `copyright.baseYear` | NONE          | The base year for the copyright notices (site-wide default, override on page-basis). |
| `copyright.entity`   | NONE          | The entity to use in copyright notices (site-wide default, override on page-basis).  |
| `copyright.license`  | NONE          | The license to use in copyright notices (site-wide default, override on page-basis). |
| `urls.github`        | NONE          | The URL for the GitHub link in the menubar.                                          |
| `urls.mastodon`      | NONE          | The URL for the Mastodon link in the menubar.                                        |

## Custom Page Parameters

| Parameter             | Default Value         | Description                                                                   |
| ---                   | ---                   | ---                                                                           |
| `book-style`          | `false`               | Format text in a more book-like manner.                                       |
| `math`                | `false`               | Load MathJax to display math on the page.                                     |
| `table-of-contents`   | `false`               | Show a table of contents at the beginning of a page.                          |
| `word-count`          | `false`               | Show the rough amount of words on a page at its beginning.                    |
| `reverse-next-prev`   | `false`               | (On section index) Reverse direction of next/prev navigation of child pages.  |

## Necessary Pages

The following three top-level pages should always exist, as they are
hard-referenced from multiple places:

| Link                  | Description                                                                    |
| ---                   | ---                                                                            |
| `/subscribe/`         | A page containing instructions on how to subscribe to updates on the site.     |
| `/contact/`           | A page containing contact information.                                         |
| `/legal-information/` | A page containing legal information like the copyright and the privacy policy. |

## Note on the `blog` Section

The `blog` section doesn't *technically* have to exist when using this template,
but the general assumption is that it does. It is where the RSS and Atom
templates pull the posts from.

## Configuration Merge

The configuration settings potentially relevant for merging in `hugo.toml` are
within:

* `[markup.highlight]`
* `[outputFormats.rss]`
