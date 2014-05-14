get-on-board, Contains scripts to be used by the Developer to setup the work
environment with favorite tools in one single step.

Like, you run a script and you get your favorite editor, programming
language, version control system, organized workspace layout etc..
created & installed in one single shot.

No `sudo apt-get install vim` or `git` or `svn` or `python`.
Just run, `get-on-board.sh` and grab a cup of coffee!

`get-on-board.sh` will be driven through a configuration file,
Configure what you want in that file and run get-on-board.sh to install
what you have configured.

Background
---
Inspiration : [Boxen Slide 37](https://speakerd.s3.amazonaws.com/presentations/5065e2abe64bdf0002011631/boxen.pdf)

Goal
---
Setting up the below things by running one single command.

```sh
curl -s http://onboard.domain.com/get-on-board.sh > /tmp/gob.sh && bash /tmp/gob.sh
```

And this would install the below stuff on your workstation(only linux for now):

    Languages
        Python
            specific 2.6 and 2.7
        Java
            v8
            Apache Tomcat
    Editors/IDEs
        Sublime, Vim, Emacs, PyCharmCE, Eclipse
    Buildtools
        Buildout, Virtualenv, Pip, Pyenv
    Browsers
        specific Firefox and Chrome (with a bunch of addons/extensions)
    Miscellaneous tools
        Setting up ssh-keys
        Git
        Configuring dotfiles
        Terminator
        Citrix Client
        Vmware
        Sqliteman
        Pomodoro Indicator
        Zeal docs

1. That `get-on-board.sh` file will be hosted under a `go` server
2. Once we run the `get-on-board.sh` file, it downloads the go binary
3. once `go` is installed, each task is performed

Incremental release plan
---
1. Install [pyenv](https://github.com/yyuu/pyenv) using Go
