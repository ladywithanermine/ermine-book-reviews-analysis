- [Project Title](#project-title)
  - [Description](#description)
  - [Getting Started](#getting-started)
    - [Dependencies](#dependencies)
  - [Getting Started](#getting-started-1)
  - [Authors](#authors)
  - [Version History](#version-history)
  - [License](#license)
  - [Acknowledgments](#acknowledgments)
# Project Title

Book details exploratory data analysis with data scraped from several sources, mostly Spanish sites.

## Description

This repo uses book information scraped from [Todos tus libros](http://www.todostuslibros.com) and other sources of book information. If you want to know more about how the data has been scraped, check my other repo [ermine-book-data-scraping](https://github.com/ladywithanermine/ermine-book-data-scraping).

## Getting Started

### Dependencies

This repo uses a pipenv virtual environment, so you'd either install pipenv and recreate the environment through the Pipfile, or you install a few python packages to be able to run the notebooks:

* jupyter (or jupyterlab)
* pandas
* matplotlib
* seaborn
* plotly

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Recreate the pipenv virtual environment using:
```
 pipenv sync --dev
```
3. Raw Data is being kept [here](/data) within this repo.

    The data as a json file is generated through the scrapy crawler in [ermine-book-data-scraping](https://github.com/ladywithanermine/ermine-book-data-scraping).
    
4. Data processing/transformation notebooks are being kept [here](/notebooks).

## Authors

[@ladywithanermine](https://github.com/ladywithanermine)

## Version History

<!--* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release-->

## License

This project is licensed under the Creative Commons License - see the LICENSE.md file for details

## Acknowledgments

<!--Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)
-->