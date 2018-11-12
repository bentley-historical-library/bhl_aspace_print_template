# BHL ArchivesSpace Print Template
This ArchivesSpace plugin adds a `print.css` stylesheet to the ArchivesSpace application that improves the formatting of records, primarily accession records, printed from the ArchivesSpace staff interface.

## Directory Structure

    frontend\
        assets\
            print.css
        views\
            layout_head.html.erb

## How It Works
The file at `frontend/views/layout_head.html.erb` links to a CSS stylesheet at `frontend/assets/print.css` with a `@media` rule of print, enabling the `print.css` stylesheet to be used when printing any record from the ArchivesSpace staff interface. The `print.css` stylesheet makes a number of formatting changes, specifically designed for accession records, that improve the layout of a page when printing from the browser.

The most notable formatting changes made by the stylesheet include:

* Expanding collapsed panels
* Setting `display` to `none` for a number of sections that are either unused by the Bentley (e.g., assessments) or not necessary to include on a printed page (e.g., the ArchivesSpace header, footer, and sidebar)
* Bolding field labels for improved readability

