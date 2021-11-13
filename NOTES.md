pip3 install virtualenvwrapper --user
export PATH=~/Library/Python/3.9/bin:$PATH
export VIRTUALENVWRAPPER_PYTHON=$(which python3)
source ~/Library/Python/3.9/bin/virtualenvwrapper.sh
mktmpenv
pip3 install gigalixir homebrew-pypi-poet
poet gigalixir
deactivate

# make sure CLI has a v1.2.3 tag and release here
# https://github.com/gigalixir/gigalixir-cli/releases

# modify gigalixir.rb
# modify the url and sha256
# to get the sha256
curl -O https://github.com/gigalixir/gigalixir-cli/archive/v1.2.3.tar.gz -L
sha256sum v1.2.3.tar.gz 

