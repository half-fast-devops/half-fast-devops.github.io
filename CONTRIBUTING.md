# Contributing to Half Fast Notes

First off, thanks for wanting to contribute! This is a small project, and we love to see people getting involved.

## Contribution Workflow

1.  **Fork the repository** to your own GitHub account.
2.  **Create a new branch** for your changes (e.g., `git checkout -b my-awesome-feature`).
3.  **Make your changes** and commit them with a clear message.
4.  **Push your branch** to your fork.
5.  **Submit a pull request** to the main repository.

## Adding a New Page

1.  Create a new `.md` file in the root directory (e.g., `my-new-page.md`).
2.  Add the following front matter to the top of the file:

    ```yaml
    ---
    layout: default
    title: My New Page Title
    ---
    ```

3.  Add your content below the front matter using Markdown. You can use the existing pages (`index.md`, `about.md`) as examples.
4.  To add a link to your new page in the navigation, edit `_layouts/default.html` and add a link in the `<nav>` section.

## Adding a New Entry (Card)

The pages are made up of "cards." To add a new card to a page:

1.  Open the `.md` file for the page you want to edit (e.g., `index.md`).
2.  Find the `<section class="zine-columns">` tag.
3.  Add a new `<article>` with the class `zine-card` and your content. You can also use the `torn` or `halftone` classes for different visual styles.

    ```html
    <article class="zine-card">
      <h3>My New Card Title</h3>
      <p>My new card content.</p>
    </article>
    ```

## Running the Site Locally

To preview your changes locally, you'll need to have Jekyll installed.

1.  Clone the repository.
2.  Install the dependencies: `bundle install`
3.  Run the Jekyll server: `bundle exec jekyll serve`
4.  Open your browser to `http://localhost:4000`.
