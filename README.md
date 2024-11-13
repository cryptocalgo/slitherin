# Slitherin by Pessimistic.io

## Installation Process

### Using Git

To install Pessimistic Detectors:

1. Install the [original Slither](https://github.com/crytic/slither#how-to-install);
2. Clone our repository;
3. Run the following command in our repository folder to add new detectors to Slither:

```bash
python3 setup.py develop
```

> Keep in mind that you don't have to reinstall the plugin after changes in the repository! 4. Dependencies must be installed in order to test the detectors on our test contracts:

```bash
npm install
```

### Using Pip

1. Install the [original Slither](https://github.com/crytic/slither#how-to-install);
2. Install the pip [package](https://pypi.org/project/slitherin/):

```bash
pip install slitherin
```

### Using Pipx

1. Install the pip [package](https://pypi.org/project/slitherin/):

```bash
pipx install slitherin
```

2. Add slitherin's bin to path:

```bash
echo -e "# Slitherin with pipx\nexport PATH=\"\$PATH:/home/$USER/.local/pipx/venvs/slitherin/bin\"\n" >> ~/.bashrc \
&& source ~/.bashrc
```

## Usage

### Slitherin-cli (Recommended)

Use Slitherin-cli to run detectors on a Hardhat/Foundry/Dapp/Brownie application. You have the following options:

- Run ONLY Slitherin detectors:

```bash
slitherin . --pess
```

- Run ONLY Slither detectors:

```bash
slitherin . --slither
```

- Run Slither detectors, then Slitherin detectors:

```bash
slitherin . --separated
```

- Run Arbitrum-specific Slitherin detectors:

```bash
slitherin . --arbitrum
```

> Keep in mind that Slitherin-cli supports all Slither run options.

### Slither

Slitherin detectors are included into original Slither after the installation. You can use Slither [as usual](https://github.com/crytic/slither#usage).
