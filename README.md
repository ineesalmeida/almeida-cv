# Almeida CV Theme

Theme to build a customizeable printable HTML/CSS CV.

![Screenshot](images/screenshot-full.png)

# Features

- Online CV with minor responsiveness
- Printable as A4 PDF
- HTML5 + CSS3
- Customizeable colors

## Print your PDF CV

When printing the page in the browser, you'll get a formatted A4 page that can be used as your PDF resume.
If your page holds more than 1 A4 page, the content will be divided into the given amount of pages.

For better formatting, you can set the number of pages in the `config.toml` file.

If badges and other elements with background don't render correctly, remember to toggle the "Background Graphics" option in the print dialog.

# Usage

## Install Hugo (extended)

To use `almeida-cv` theme you need to install Hugo Extended by following https://gohugo.io/getting-started/installing/.

## Create your personal website

```
hugo new site <your website's name>
cd <your website's name>
git init
git submodule add https://github.com/ineesalmeida/almeida-cv.git themes/almeida-cv
```

Replace the files in your site root's directory with the ones in `themes/almeida-cv/exampleSite`.

## Start Hugo in development mode

```
hugo server -D
```

Your site is now available at http://localhost:1313/.

## Customization

Your professional data should be added in the `data/content.yaml` file. You can change the theme colors and number of
pages in the `config.toml` file. For working example, see `exampleSite` directory.

### Configuration Parameters

Below are the available parameters for `config.toml` and their descriptions:

| Parameter                               | Description                                               | Example/Default        |
| --------------------------------------- | --------------------------------------------------------- | ---------------------- |
| `languageCode`                          | The language code for the site.                           | `en-us`                |
| `defaultContentLanguage`                | The default content language.                             | `en`                   |
| `enableRobotsTXT`                       | Enable generation of robots.txt.                          | `true`                 |
| `enableEmoji`                           | Enable emoji support.                                     | `true`                 |
| `theme`                                 | The theme to use.                                         | `almeida-cv`           |
| `disableKinds`                          | List of page types to disable (e.g., RSS, sitemap, etc.). | See example            |
| `baseURL`                               | The base URL of the site.                                 | `https://example.com/` |
| `title`                                 | The title of the site.                                    | `Example - CV`         |
| `params.enableMetaTags`                 | Enable meta tags for SEO.                                 | `true`                 |
| `params.colorLight`                     | Light color for theme.                                    | `#fff`                 |
| `params.colorDark`                      | Dark color for theme.                                     | `#666`                 |
| `params.colorPageBackground`            | Background color for the page.                            | `#ddd`                 |
| `params.colorPrimary`                   | Primary color for highlights.                             | `#e3bfb8`              |
| `params.colorSecondary`                 | Secondary color for highlights.                           | `#aaa`                 |
| `params.colorIconPrimary`               | Primary color for icons.                                  | `#fff`                 |
| `params.colorIconBackground`            | Background color for icons.                               | `#e3bfb8`              |
| `params.colorRightColumnBackground`     | Background color for the right column.                    | `#f5f5f5`              |
| `params.colorRightColumnHeadingText`    | Heading text color in the right column.                   | `#666`                 |
| `params.colorRightColumnBodyText`       | Body text color in the right column.                      | `#666`                 |
| `params.colorRightColumnIconPrimary`    | Primary color for icons in the right column.              | `#fff`                 |
| `params.colorRightColumnIconBackground` | Background color for icons in the right column.           | `#e3bfb8`              |
| `params.pages`                          | Number of A4 pages to use for the CV.                     | `1`                    |
| `params.swapColumns`                    | If `true`, swaps the left and right columns.              | `false`                |
| `params.footerNote`                     | Text to display in the footer.                            | See example            |

Add or adjust these parameters in your `config.toml` to customize your CV's appearance and behavior.

For more advanced customization, in your site root directory create `assets/scss/_custom.scss` file where you can
overwrite theme SCSS as per your liking.

## Building

To generate static files of your website, execute the following:

```
hugo --minify
```

within the root of your project.

# Contributing

Post bugs and contributions to the issue tracker. Or make a pull request.
