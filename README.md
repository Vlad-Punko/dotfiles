# workstation

```bash
echo "${HOME} sweet ${HOME}"
```

## Installation

```bash
# Step -- 1.
sudo softwareupdate --all --install

# Step -- 2.
xcode-select --install
xcode-select --print-path

# Step -- 3.
/bin/bash -c "$(curl -sSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Step -- 4.
git clone --depth=1 --branch=master https://github.com/vladpunko/workstation.git

# Step -- 5.
cd ./workstation/playbook

# Step -- 6.
python3 -m venv .venv && source ./.venv/bin/activate

# Step -- 7.
python3 -m pip install --requirement=requirements.txt

# Step -- 8.
ansible-playbook --ask-become-pass --inventory=hosts workstation.yml
```

## License

[MIT](https://choosealicense.com/licenses/mit)
