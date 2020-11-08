pip3 install virtualenvwrapper --user
export PATH=~/Library/Python/3.7/bin:$PATH
export VIRTUALENVWRAPPER_PYTHON=$(which python3)
source ~/Library/Python/3.7/bin/virtualenvwrapper.sh
mktmpenv
pip3 install gigalixir homebrew-pypi-poet
poet gigalixir
deactivate
