# alexmpdx QuPath Extensions — catalog

A [QuPath](https://qupath.github.io/) **extension catalog** for QuPath extensions by
alexmpdx. Adding it lets QuPath browse, install and update these extensions directly
from *Extensions → Manage extensions*.

## Add this catalog to QuPath

1. In QuPath (0.7+): **Extensions → Manage extensions**.
2. Click **Add catalog** (the **+** button).
3. Paste this repository's URL:
   ```
   https://github.com/alexmpdx/qupath-catalog-alexmpdx
   ```
4. The extensions below will appear, ready to install.

## Extensions in this catalog

| Extension | Description | Repo |
| --- | --- | --- |
| **Smooth Annotation** | Inkscape-style smoothing & simplification of annotation outlines (Bézier / Chaikin / Catmull-Rom) with corner preservation and a live preview. | [qupath-extension-smooth-annotation](https://github.com/alexmpdx/qupath-extension-smooth-annotation) |
| **Active Image Helper** | Highlights the active image in the project list with a distinct color, and adds right-click actions to scroll to or remove the current image. | [qupath-extension-active-image-helper](https://github.com/alexmpdx/qupath-extension-active-image-helper) |

## Catalog format

`catalog.json` follows the [QuPath extension catalog](https://github.com/qupath/qupath-catalog)
schema: a top-level `name`, `description`, and an `extensions` array. Each extension has
`name`, `description`, `author`, `homepage`, optional `starred`, and a `releases` array;
each release has `name` (tag), `main_url` (the jar), optional `javadoc_urls` /
`optional_dependency_urls`, and a `version_range` (`min` / optional `max` QuPath version).

To add a new release, append an entry to that extension's `releases` array (newest first);
to add a new extension, append to `extensions`.
