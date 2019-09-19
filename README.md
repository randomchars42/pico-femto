A very minimal theme for [Pico CMS](https://www.picocms.org), designed to help
simple blogs.

## Installation

For Pico CMS > 2.0:

  * Download or clone the code and upload it to `themes/femto`.
  * Edit `config/config.yml`, change:
    ```
		theme: default
    ```

		to

    ```
		theme: femto
    ```
  * That's it!

## Demo

  * You can find a live demo at <http://blog.pixelwoelkchen.de>

## Usage

### Structure

For things like Impressum just create a file `/impressum.md`.

Blog content goes into subfolders, either a single folder, e.g. `/blog/` or one
folder per topic. Make sure every folder has an `index.md` with **optional**
content (the theme will automagically display all posts as links).

So your folder structure may look like:

```
/index.md
/impressum.md
/blog/index.md
/blog/my_latest_craze.md
/blog/a_fancy_idea.md
/blog/my_first_post_sigh.md
...
```

or

```
/index.md
/impressum.md
/ideas/index.md
/ideas/my_latest_craze.md
/ideas/a_fancy_idea.md
/ideas/my_first_post_sigh.md
/notsobrilliant/index.md
/notsobrilliant/don_t_do_this.md
...
```

Content in a folder called `archive` will not be listed on the front page.

### Ordering first level pages

By default, the pages on the first level appear in alphabetical order in your navigation. If you wanted to change that behaviour you need to edit `config/config.yml` so it looks like this:

```
pages_order_by_meta: order
pages_order_by: meta
```

Now you can add an `Order: NUMERICALVALUE` to each YAML-Header on your first level pages, *e.g.*:

```
/*
Title: Archive
Author: Eike Kühn
Date: 19 September 2019
Order: 3
*/

Old stuff
```
