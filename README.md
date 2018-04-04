# Spacetime
A gorgeous and simplistic Jekyll theme spacetime for multiple blogging categories in one space. Checkout the demo [here](https://techcentaur.github.io/space/).

![spacetime screenshot web](https://github.com/techcentaur/spacetime/blob/master/img/space1.jpg)

## Features
- Compatible with GitHub Pages
- Responsive design (looks just as good on mobile)
- Multiple pagination of posts depending on categories and subjects.
- More than one blog maintainence system
- Syntax highlighting, with the help of Pygments
- Markdown and HTML text formatting


## Usage
### 1. Fork and Clone
Fork this repository then clone it.

### 2. Install dependencies
Spacetime uses Jekyll's built-SCSS compiler to generate CSS. You'll need to install the Jekyll gem:

```bash
$ gem install jekyll
$ gem install jekyll-paginate-multiple

```

### 3. Create your site
Edit the `_config.yml` file to suit your site. Also replace posts and content with your own.

### 4. Running Locally
To test your site locally, run this in your site's root directory

```bash
$ jekyll serve
```
Head to http://localhost:4000/space/ or http://127.0.0.1:4000/space/ to see your site in action.


## Help
### Using Multi-Pagination

Edit the `_config.yml` file with changing the directories of the differnet blogs with there pagination counts and supporting urls as

```yaml

paginate_multiple:
  - paginate: 5
    paginate_path: '/blog/page:num/'
    sub_dir: '/blog'
  - paginate: 5
    paginate_path: '/writings/page:num/'
    sub_dir: '/writings'
  - paginate: 10
    paginate_path: '/quotes/page:num'
    sub_dir: '/quotes'


```

Also, make different folders in the _posts folder to put up your blog-posts. You also need to make their individual home pages since they will be shown on different index files.

## Contributing
Found a bug or have a suggestion? Feel free to create an issue or make a pull request!


