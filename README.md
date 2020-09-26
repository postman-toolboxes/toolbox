# Postman API Toolbox
This is an open source template for a toolbox that can be used to deploy API resource centers. This template was originally developed as part of Postman's COVID-19 Resource Center, and then further evolved to be a general template that could be used to deploy a variety of API resources centers. Helping provide single landing pages for a variety of topics, industries, and trends, where developers can find what they need to develop applications.

## Single Page Application
A Postman API toolbox is a Jekyll powered single page applications that uses an APIs.yaml file as it's core data source. The purpose of an API toolbox is to not just publish a listing of APIs available for developers to use in applicaitons, but also encourage API submissions from the community. Here are the core technologies at play in this Postman API toolbox.

- [**GitHub**](https://github.com/) - These API toolboxes can be run 100% on GitHub and do not need any outside hosting or APIs to make them work.
- [**GitHub Pages**](https://pages.github.com/) - The project hosting layer to GitHub, allowing simple project sites to be hosted using a GitHub repository.
- [**Jekyll**](https://jekyllrb.com/) - The content in these API toolboxes is managed using a static site content management system called Jekyll.
- [**APIs.yaml**](http://apisyaml.org/) - The data source for these API toolboxes is made available via a YAML file that uses a standard called APIs.yaml, providing a machine readable index of aPIs.

These single page application API toolboxes are designed to run 100% on GitHub, and be updated using Git commits or using the GitHub API. Allowing all APIs to managed via a single APIs.yaml core, and displayed as a single page application using Jekyll, with the hosting environment being GitHub, and GitHub pages. Working to keep the number of folders and files needed to operate each site as minimal as possible, with hosting free.

## Site Structure
The site uses a minimal structure to help publish the single page application, keeping the data and the presentation layer as simple and effective as possible. Here is a breakdown of the site outline for operating each API toolbox:

- **_data** - The central data store for the site.
  - **apis.yaml** - The APIs.yaml file of all APIs.
- **_includes** - Individual files used to display data.
  - **api-by-tag-listing.html** - Lists all APIs by tag.
  - **api-listing.html** - Lists all of the APIs.
  - **api-tag-anchors.html** - Provides a list of tags as links.
  - **spec-listing.html** - Lists all of the specifications.
  - **tag-listing.html** - Lists all of the tags across aPIs.
  - **tool-listing.html** - Lists all of the open source tools.
  - **visualization-listing.html** - Lists the visualizations for APIs.
- **_layouts** - The three types of page layouts available.
  - **default.html** - The default layout for each page.
  - **none-html** - When you want to display JSON data.
  - **post.html** - The template that should be used for each blog psot.
- **_posts** - Where each blog post update for a project goes.
- **_config.yml** - The configuration file for the Jekyll site.
- **apis.json** - A generated APIs.json from the APIs.yaml file.
- **index.html** - The home page for the single page application.
- **LICENSE** - The license for the project and it's data.
- **README.md** - The README for the API toolbox project.

You are not required to use all the includes in your index.html for each page, but should provide a diverse range of use cases for displaying relevant API operational data using the APIs.yaml index. Visit the Jekyll site to learn more about the Liquid syntax being used to display the YAML data, or visit the [Liquid template language documentation](https://shopify.github.io/liquid/).
