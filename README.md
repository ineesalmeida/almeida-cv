# Almeida CV Theme
Theme to build a customizeable printable HTML/CSS CV.

![Screenshot](images/screenshot-full.png)

# Features
 - Online CV with minor responsiveness
 - Printable as A4 PDF

# Download 
Clone the repo: `git clone https://github.com/ineesalmeida/almeida-cv`

# Installation
## Install Hugo
To use almeida-cv theme you need to install Hugo by following https://gohugo.io/getting-started/installing/.

## Create your personal website and run
```
hugo new site <your website's name>
cd <your website's name>/themes/
```
Clone the theme (`git clone https://github.com/ineesalmeida/almeida-cv`).
Replace the "config.toml" file that in the project's root directory with `themes/almeida-cv/exampleSite/config.toml`.
Replace the "content.yaml" file that in the project's root directory with `themes/almeida-cv/exampleSite/data/content.yaml`.
```
hugo server -D
```
The theme is alive on http://localhost:1313/ 

## Customization
You can change the theme colors in the `config.toml` file.
Your professional data should be added in the `data/content.yaml`.

# Building 
To generate your site in the public folder, execute the following:
```
hugo
```
within the root of your project.


# Contributing 
Post bugs and contributions to the issue tracker. Or make a pull request.

# License 
This template is 100% FREE as long as you keep the footer attribution link. You do not have the rights to resell, sublicense or redistribute (even for free) the template on its own or as a separate attachment from any of your work. If you’d like to use this template without the footer attribution link, you can buy the commercial license. Send an email to contact@ines-almeida.com.