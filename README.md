# heroku-buildpack-vim

Heroku Buildpack to install [Vim](https://www.vim.org/)

> Vim - the ubiquitous text editor


## How it works

Installs from Amazon S3 using a statically linked [Vim binary]((https://s3.amazonaws.com/bengoa/vim-static.tar.gz)).
Vim instalation ends in `/app/vim` directory.

## Configure from CLI

```bash
heroku buildpacks:add https://github.com/carloluis/heroku-buildpack-vim
```

## Configure from app manifest

```json
{
    "buildpacks": [
        {
            "url": "https://github.com/carloluis/heroku-buildpack-vim"
        }
    ]
}
```

## License

MIT © [Carloluis](https://github.com/carloluis)
