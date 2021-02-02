## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/compsciencelab/compscience-org/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Local Installation

Follow the instructions [here](https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll) to install dependencies

Clone this repo, navigate to `docs` directory, and run `jekyll serve`

Navigate to the server address, and everything should be set.

While struggling to get this running, I also followed instructions [here](https://kbroman.org/simple_site/pages/local_test.html). So if the above doesn't work, try following that one as well.

### General Method for Quick Styling

Once I have a local server running, I generally test CSS changes using the Chrome Development Tools (right-click > Inspect) because the changes are instantaneous.

Once I've got things looking how I want, I copy the new CSS rules over to `style.scss`, add a good selector (like the element-type and class), and reload and refresh the local server to make sure it worked.

### Directory Layout

The entire site is contained in the `docs` directory.

Within `docs`:
- `_data`: YAML files with text used to populate sections of the home page, header, or footer. For example, `apply.yml` contains text used to populate the Apply section of the home page. Text for the generic two-column layout is not populated from `_data`.
- `_includes`: HTML layouts for sections of the home page. For example, `apply.html` is the layout used for the Apply section of the home page. It also contains the Markdown files used to populate the two-column layout.
- `_layouts`: HTML layout for the home page, the header and footer layout, and layout for the positions page
- `assets`: CSS styles and images
- `_config.yml`: Site theme and title
- `CNAME`: Site URL
- `index.html`: Landing page, just references the `home` layout
- `positions.md`: Markdown content of the Positions page
- `publications.html`: HTML content of the Publications page

### Copying the two-column layout

To make the second column  section (for example), copy and paste (or rename, if first two-column section) `two_column1_column1.md`, `two_column1_column2.md`, and `two_column1.html` in the `_includes` directory. Change the names of the files, but keep some identifier in the Markdown filenames for which column is which. Change the Markdown filenames in the corresponding HTML file (originally `two_column1.html`). You can place the two-column section anywhere you want on the Home page by adding an `{% includes ... %}` statement there. Then you can edit the contents of the columns by editing the Markdown files from earlier.


### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/compsciencelab/compscience-org/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
