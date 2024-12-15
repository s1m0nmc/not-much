<a id="readme-top"></a>

# Not Much

`not-much` is a minimal Hugo theme that I use for my personal website. It doesn't have any fancy shortcode or useless feature.

**It's basic, simple and minimal.**

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Prerequisites

- Git
- Hugo

### Installing

Clone this repository in your machine:

```shell
$ git clone https://github.com/imgios/not-much.git
```

Change the workdir to `not-much/exampleSite` and start the Hugo server:

```shell
$ cd not-much/exampleSite
$ hugo server -D
hugo server -D
Watching for changes in \not-much\{archetypes,assets,exampleSite,i18n,layouts,static}
Watching for config changes in \not-much\exampleSite\config.toml
Start building sites …
...
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

Now you are ready to update the theme and see the changes live @ [localhost](http://localhost:1313/).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Deployment

The theme can be installed in two different ways:

1. By adding `not-much` as submodule in your Hugo website repository

```shell
$ cd your-hugo-website
$ git submodule add https://github.com/imgios/not-much.git themes/not-much
```

2. By adding the `not-much` theme dir in `/your-hugo-website/themes/*`

The first option is quite limited as you won't be able to edit the templates if you wanted to. The second option, on the other hand, gives you the entire structure of the theme and allows you to customise it as you wish.

Once done, update (or add) the `theme` parameter in your website configuration file to `theme = not-much`.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Configuration

You can update the website index, menu and copyright directly in your Hugo site `config.toml`.

A reference can be found in [`exampleSite/config.toml`](https://github.com/imgios/not-much/blob/dev/exampleSite/config.toml)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Homepage

You can update the homepage by creating the index in `your-hugo-wesbite/content/_index.md` with the following structure:

```yaml
---
heading: "not much 👋🏻"
lead: "A minimal theme for Hugo"
description: "This is a not-much demo, built with Hugo. Explore it to see what not-much is offering."
---
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Menu items and custom links

The main menu can be customised as you prefer to add site-related locations (e.g., your blog location) or your social links:

```toml
# Controls the navigation
[[menu.main]]
  identifier = "about"
  name = "about"
  title = "About"
  url = "/"

[[menu.main]]
  identifier = "posts"
  name = "posts"
  title = "Posts"
  url = "/posts"

[[menu.main]]
  identifier = "github"
  name = "github"
  title = "GitHub"
  url = "https://github.com/imgios"
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

#### Copyright

Write your custom copyright notice in the footer by updating the `copyright` field:

```toml
copyright = "© {year}"
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Built With

* [Hugo](https://gohugo.io/) - The static site generator framework
* [Bootstrap](https://getbootstrap.com/) - Free and open-source CSS library
* [RedHat Mono Font](https://fonts.google.com/specimen/Red+Hat+Mono) - Used as theme font

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

<!-- Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us. -->
Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".

1. [Fork the project](https://github.com/imgios/not-much/fork)
2. Create your Feature Branch (`git checkout -b feat/cool-feature`)
3. Commit your Changes (`git commit -m 'add some cool-feature'`)
4. Push to the Branch (`git push origin feat/cool-feature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/imgios/not-much/tags). 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

<p align="right">(<a href="#readme-top">back to top</a>)</p>