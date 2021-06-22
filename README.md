- [:books: Book data exploratory analysis](#books-book-data-exploratory-analysis)
  - [Business case](#business-case)
  - [Getting Started](#getting-started)
    - [Dependencies](#dependencies)
    - [Setup](#setup)
  - [Authors](#authors)
  - [Version History](#version-history)
  - [License](#license)
  - [Acknowledgments](#acknowledgments)
# :books: Book data exploratory analysis

Book details exploratory data analysis with data scraped from several sources, mostly Spanish sites.

## Business case

I am a book lover and, most of all, I am passionate about fiction. [Literary fiction](https://en.wikipedia.org/wiki/Literary_fiction#:~:text=Literary%20fiction%20is%20a%20term,commercial%20or%20%22genre%22%20fiction.&text=Furthermore%2C%20the%20study%20of%20genre,within%20academia%20in%20recent%20decades.) in particular, though not only. So I decided this interest of mine could be the spark for a data science pet project, where I could build the end-to-end ETL and analysis pipelines and extract some interesting insights about books, apart from reading (and enjoying) them.

There are few book-related datasets around. Some are in [Kaggle](https://www.kaggle.com/datasets), such as [this one](https://www.kaggle.com/sootersaalu/amazon-top-50-bestselling-books-2009-2019) or [this other one](https://www.kaggle.com/tanguypledel/science-fiction-books-subgenres). They are mostly related to genre fiction or Amazon book data... in English. I have found no datasets related to books solely in Spanish or to the Spanish book market, so I decided to gather the data by myself and learn a few new things in the process.

The selection of suitable sites to retrieve book data for books published in Spain is quite reduced, more so since the [Goodreads API](https://www.goodreads.com/api) was deprecated in December 2020. Among the available ones, the most straightforward is [Todos tus libros](http://www.todostuslibros.com), a site put up by [Cegal](https://www.cegal.es/), the Spanish bookshops association, to publicize books and their availability, as part of a campaign to encourage readers to buy locally. The site (as stated in the ['Who we are'](https://todostuslibros.com/servicios/quienes_somos) section) includes information (sometimes incomplete) on more than 4 million books --and counting.

The site allows searches on author, title, publishing house, ISBN or date of publication and books are tagged for one or more categories ('materias'). Initially, I have chosen for the exploratory analysis the category related to literary fiction: ['Ficción moderna y contemporánea'](http://www.todostuslibros.com/materia/ficcion-moderna-y-contemporanea_FA), containing about 100,000 books. The books details were scraped and formatted in a JSON file, including the following information:

* Title
* Authors
* Publisher
* Price (if available)
* Publishing country
* Publishing language
* Original language
* ISBN
* EAN
* Publication date
* Type of binding
* Number of pages
* Number of bookstores where the book is available (at the time of the dataset generation)
* Tags: a compendium of genre, language, style, etc.
* Book cover URL

For exhaustive details about the scraping process, please check my repo [ermine-book-data-scraping](https://github.com/ladywithanermine/ermine-book-data-scraping). 

## Getting Started

### Dependencies

This repo uses a pipenv virtual environment, so you'd either install [pipenv](https://pipenv-es.readthedocs.io) and recreate the environment or you may install a few python packages in your python environment of choice to be able to run the notebooks and the rest of the code:

* jupyter (or jupyterlab)
* pandas
* matplotlib
* seaborn
* plotly

### Setup

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

* [An inspirational post on how to setup a professional data science repository](https://towardsdatascience.com/how-to-create-a-professional-github-data-science-repository-84e9607644a2)
<!--Inspiration, code snippets, etc.
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)
-->