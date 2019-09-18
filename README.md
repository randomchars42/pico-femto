A very minimal theme for [Pico CMS](https://www.picocms.org), designed to help simple blogs.

## Installation

For Pico CMS > 2.0:

  * Download or clone the code and upload it to `themes/femto`.
  * Edit `config/config.yml`:
    ```
		theme: femto
    ```
  * That's it!

## Demo

  * You can find a live demo at <blog.pixelwoelkchen.de>

## Usage

`femto` supports two sorts of content:

  * Files at top level ('/index.md', '/contact.md', etc.) will be permanently visible for navigation (like `start`, `impressum`, etc)
  * (Blog-) content goes into subfolders, either:
      * a folder like `blog` for everything you post, or
      * different folders, the folder names can be seen as "tags", each folder should have an `index.md` with **optional** content.
