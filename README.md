## <p align="center">Project 3</p>

<p align="center"><img src="https://komarev.com/ghpvc/?username=LauraW-code&color=blueviolet&style=for-the-badge"></p>

# AFAC 974

This project was my third collaborative project during the web developper course with Wild Code School.

Its goal was to create an online art gallery for a cultural association, using PHP and the framework Symfony.

I endorsed the role of Product Owner on this project and it was very enriching and forced me to improve my organisation skill.

### :hammer_and_wrench: Technologies and tools: 

<div>
  <img src="https://github.com/devicons/devicon/blob/master/icons/php/php-original.svg" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-original.svg" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/symfony/symfony-original-wordmark.svg" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/mysql/mysql-original-wordmark.svg" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/bootstrap/bootstrap-original.svg" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/trello/trello-original.svg" width="40" height="40"/>&nbsp;
</div>

## Change Log
See [CHANGELOG.md](CHANGELOG.md) for more information.

## Presentation

This starter kit is here to easily start a repository for Wild Code School students.

It's symfony website-skeleton project with some additional library (webpack, fixtures) and tools to validate code standards.

* GrumPHP, as pre-commit hook, will run 2 tools when `git commit` is run :

    * PHP_CodeSniffer to check PSR12
    * PHPStan focuses on finding errors in your code (without actually running it)
    * PHPmd will check if you follow PHP best practices

  If tests fail, the commit is canceled and a warning message is displayed to developper.

* Github Action as Continuous Integration will be run when a branch with active pull request is updated on github. It will run :

    * Tasks to check if vendor, .idea, env.local are not versionned,
    * PHP_CodeSniffer, PHPStan and PHPmd with same configuration as GrumPHP.

## Getting Started for Students

### Prerequisites

1. Check composer is installed
2. Check yarn & node are installed

### Install

1. Clone this project
2. Run `composer install`
3. Run `yarn install`
4. Run `yarn encore dev` to build assets

### Working

1. Run `symfony server:start` to launch your local php web server
2. Run `yarn run dev --watch` to launch your local server for assets (or `yarn dev-server` do the same with Hot Module Reload activated)

### Testing

1. Run `php ./vendor/bin/phpcs` to launch PHP code sniffer
2. Run `php ./vendor/bin/phpstan analyse src --level max` to launch PHPStan
3. Run `php ./vendor/bin/phpmd src text phpmd.xml` to launch PHP Mess Detector

### Windows Users

If you develop on Windows, you should edit you git configuration to change your end of line rules with this command:

`git config --global core.autocrlf true`

The `.editorconfig` file in root directory do this for you. You probably need `EditorConfig` extension if your IDE is VSCode.

### Run locally with Docker

1. Fill DATABASE_URL variable in .env.local file with
`DATABASE_URL="mysql://root:password@database:3306/<choose_a_db_name>"`
2. Install Docker Desktop an run the command:
```bash
docker compose up -d
```
3. Wait a moment and visit http://localhost:8000


## Deployment

Some files are used to manage automatic deployments (using Docker, GitHub Action to a Traefik environment). Please do not modify them.

* [docker-compose.yml](/docker-compose.yml) Docker configuration for local development
* [docker-compose.prod.yml](/docker-compose.prod.yml) Docker configuration for production
* [.github/workflows/deploy-traefik.yml](/.github/workflows/deploy-traefik.yml) GitHub Action workflow to deploy Traefik
* [Dockerfile](/Dockerfile) Web app configuration for Docker container
* [docker-entry.sh](/docker-entry.sh) shell instruction to execute when docker image is built
* [nginx.conf](/ginx.conf) Nginx server configuration
* [php.ini](/php.ini) Php configuration


## Built With

* [Symfony](https://github.com/symfony/symfony)
* [GrumPHP](https://github.com/phpro/grumphp)
* [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer)
* [PHPStan](https://github.com/phpstan/phpstan)
* [PHPMD](http://phpmd.org)
* [Sass-Lint](https://github.com/sasstools/sass-lint)



## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning


## Authors

Wild Code School trainers team

## License

MIT License

Copyright (c) 2019 aurelien@wildcodeschool.fr

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Acknowledgments

