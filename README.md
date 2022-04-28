# coffee-web-frontend

## Build Setup

```bash
# 
$ cd source

# create env file

$ cp .env-example .env

# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start


```

### How to use github
```bash
# pull project from develop branch
$ git init
$ git remote add origin <git link>
$ git pull origin develop

# or
$ git clone <git link>
$ cd <file name>
$ git pull origin develop

# push code to another branch except develop branch and master branch

#create branch 
$ git branch <branch name>
$ git checkout <branch name>

#push code

$ git add .
$ git commit -m "message"
$ git push origin <branch name EXCEPT develop and master branch>

# create pull request from github.com frm <branch name> to <develop> not <master>
```
## Folder Structure
```

|– components/
|   |-Header.vue            # Header component
|
|– pages/
|   |– index.vue            # Home page
|   ...                     # Etc…
|- plugins/
|   |- api.js
|   ...
|
|– static/
|   |– favicon.ico          # Favicon file
|   ...                     # Etc…
|
|– store/
|   |– posts.js             # Store post
|
|- layouts/
|   |- default.vue          # default layout
|
|-styles/                   # Structure of styles
|   |
|   |– base/
|   |   |– _reset.scss       # Reset/normalize
|   |   |– _typography.scss  # Typography rules
|   |   ...                  # Etc…
|   |
|   |– components/
|   |   |– _buttons.scss     # Buttons
|   |   |– _carousel.scss    # Carousel
|   |   |– _cover.scss       # Cover
|   |   |– _dropdown.scss    # Dropdown
|   |   ...                  # Etc…
|   |
|   |– layout/
|   |   |– _navigation.scss  # Navigation
|   |   |– _grid.scss        # Grid system
|   |   |– _header.scss      # Header
|   |   |– _footer.scss      # Footer
|   |   |– _sidebar.scss     # Sidebar
|   |   |– _forms.scss       # Forms
|   |   ...                  # Etc…
|   |
|   |– pages/
|   |   |– _home.scss        # Home specific styles
|   |   |– _contact.scss     # Contact specific styles
|   |   ...                  # Etc…
|   |
|   |– utils/
|   |   |– _variables.scss   # Sass Variables
|   |   |– _functions.scss   # Sass Functions
|   |   |– _mixins.scss      # Sass Mixins
|   |   |– _helpers.scss     # Class & placeholders helpers
|   |
|   |– vendors/
|   |   |– _bootstrap.scss   # Bootstrap
|   |   ...                  # Etc…
|   |
|   |
|   `– style.scss            # Primary Sass file
|
|- nuxt.config.js            # Nuxt config file
|- package.json 
...

```


For detailed explanation on how things work, check out the [documentation](https://nuxtjs.org).

## Special Directories

You can create the following extra directories, some of which have special behaviors. Only `pages` is required; you can delete them if you don't want to use their functionality.

### `assets`

The assets directory contains your uncompiled assets such as Stylus or Sass files, images, or fonts.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/assets).

### `components`

The components directory contains your Vue.js components. Components make up the different parts of your page and can be reused and imported into your pages, layouts and even other components.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/components).

### `layouts`

Layouts are a great help when you want to change the look and feel of your Nuxt app, whether you want to include a sidebar or have distinct layouts for mobile and desktop.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/layouts).

### `pages`

This directory contains your application views and routes. Nuxt will read all the `*.vue` files inside this directory and setup Vue Router automatically.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/get-started/routing).

### `plugins`

The plugins directory contains JavaScript plugins that you want to run before instantiating the root Vue.js Application. This is the place to add Vue plugins and to inject functions or constants. Every time you need to use `Vue.use()`, you should create a file in `plugins/` and add its path to plugins in `nuxt.config.js`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/plugins).

### `static`

This directory contains your static files. Each file inside this directory is mapped to `/`.

Example: `/static/robots.txt` is mapped as `/robots.txt`.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/static).

### `store`

This directory contains your Vuex store files. Creating a file in this directory automatically activates Vuex.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/docs/2.x/directory-structure/store).



# Create .env file for config docker
```
$ cp .env.example .env
```
# Docker
```
$ docker-compose up -d --build

```

# Composer install
```
$ docker-compose exec app composer install

```
# Copy .env of app
```
$cd src

$cp .env.example .env

```
# Config DB in .env 
```
DB_CONNECTION=mysql
DB_HOST=coffee-db
DB_PORT=3010
DB_DATABASE=coffee_database
DB_USERNAME=homestead
DB_PASSWORD=secret

```

# Migrate and seed data
```
$ docker-compose exec app ash

[/work/app]

$php artisan storage:link

$php artisan key:generate

$php artisan migrate

$php artisan db:seed

```

# Access admin site in local

```
http://localhost:8888/admin

admin@gmail.com/12345678

```
