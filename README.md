# pyenv & pyenv-virtualenv

```bash
git clone https://github.com/yyuu/pyenv.git ~/.pyenv
```

```fish
# IN .config/fish/config.fish
set -x PYENV_ROOT "$HOME/.pyenv"
set -x PATH "$PYENV_ROOT/bin" $PATH
eval (pyenv init - | source)
```

```bash
sudo apt install git gcc make openssl libssl-dev libbz2-dev libreadline-dev libsqlite3-dev zlib1g-dev libffi-dev
(sudo apt install libncurses5 libncurses5-dev libncursesw5)
pyenv install 3.7.3
```

```bash
git clone https://github.com/yyuu/pyenv-virtualenv.git ~/.pyenv/plugins/pyenv-virtualenv
```

```fish
# IN .config/fish/config.fish
eval (pyenv virtualenv-init - | source)
```

```bash
pyenv virtualenv 3.7.3 hoge
```

# golang-go on ubuntu

1.12が入ってくることまで確認

```bash
sudo add-apt-repository ppa:longsleep/golang-backports
sudo apt update
sudo apt install golang-go
```
