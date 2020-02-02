# heroku-buildpack-vim &middot; [![GitHub license](https://img.shields.io/github/license/carloluis/heroku-buildpack-vim)](https://github.com/carloluis/heroku-buildpack-vim/blob/master/LICENSE)

Heroku Buildpack to install [Vim](https://www.vim.org/)

> Vim - the ubiquitous text editor

## How it works

Installs from Amazon S3 using a statically linked [Vim binary](https://s3.amazonaws.com/bengoa/vim-static.tar.gz).
Vim installation ends in `/app/vim` directory.

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
