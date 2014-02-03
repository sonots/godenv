godenv
========

Just a wrapper script of direnv, but I think this is enough


## How to install

```bash
git clone http://github.com/zimbatm/direnv
cd direnv
make install
curl https://raw.github.com/sonots/godenv/master/godenv -o /usr/local/bin/
```

## Add hook to shell

~/.zshrc
```
eval "$(godenv hook zsh)"
```

## Create a project

```
$ godenv new project
```

You will get `project` directory and `project/.envrc` file. 

As `cd` to the project, `goenvdir` (actually envdir) will loads `.envrc` and set GOPATH, etc automatically. 
