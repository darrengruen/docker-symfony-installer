# Docker Symfony Installer

For more info on the installer itself, [http://symfony.com/doc/current/book/installation.html](http://symfony.com/doc/current/book/installation.html)

Create a new Symfony application.

## Usage

```
docker run -it -rm \
    -v [path/to/install/dir]:/project \
    --name symfony-installer \
    gruen/symfony-installer \
    new [project_directory] [options]
```

Create a new Symfony 2.8 project in the current directory
```
docker run -it -rm \
    -v $(pwd):/project \
    --name symfony-installer \
    gruen/symfony-installer \
    new ./ 2.8
```
