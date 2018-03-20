# heroku-buildpack-vim

Heroku Buildpack to install [Vim](https://www.vim.org/)

> Vim - the ubiquitous text editor


## How it works

Installs Vim from [Amazon S3](https://s3.amazonaws.com/heroku-vim/vim-7.3.tar.gz).
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
