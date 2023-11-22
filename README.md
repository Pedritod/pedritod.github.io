Second, you should update icon links in `_includes/particles-home.html` and add/remove icons as needed. You might want to add icons that are not included in the theme by default. For more information on how to do this, see [this post](https://cvless.netlify.app/2022/08/01/on-the-use-of-icons/).

Third, you should customize the file `_includes/contact.html` by inputting your contact details and adding/removing lines as needed. This information is prepended to your CV.

Fourth, you might want to edit the style variables specified in `_sass/_variables.scss`. These allow you to customize the theme's color scheme and typefaces. There are many resources on the web to learn the principles of good web design. I personally recommend Matthew Butterick's [Practical Typography](https://practicaltypography.com/websites.html).

In addition to these files, you can customize favicons in the `assets` folder. For that, [favicon.io](https://favicon.io/) is an excellent tool. You can also change the particles.js configurations in `assets/json`. The [library homepage](https://vincentgarreau.com/particles.js/) features an interactive tool from which you can export a new configuration.

## Local Development

This repo includes a docker-compose file that allows you to quickly setup a container running Jekyll. If you don't already have Docker and docker-compose installed, you can install them using the following guides from Docker:

**Install Guides**
* [Docker](https://docs.docker.com/get-docker/)
* [docker-compose](https://docs.docker.com/compose/install/)

To start the container simply run:

```
docker-compose up
```

Alternatively you can run the container without docker-compose using the following command on Mac/Linux:

```
docker run -p 4000:4000 -v $(pwd):/site bretfisher/jekyll-serve
```
