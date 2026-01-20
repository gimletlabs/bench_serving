## Setup

### Prerequisites
- [pyenv](https://github.com/pyenv/pyenv#installation)
- [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv#installation) (optional but recommended)

### Installation

1. Install the required Python version:
```bash
   pyenv install $(cat .python-version)
```

2. Create and activate a virtual environment:
```bash
   pyenv virtualenv $(cat .python-version) myproject-env
   pyenv activate myproject-env
```

   Or use the built-in venv:
```bash
   python -m venv venv
   source venv/bin/activate
```

3. Install dependencies:
```bash
   pip install -r requirements.txt
```

### Quick Setup (one-liner)
```bash
pyenv install -s $(cat .python-version) && pyenv virtualenv $(cat .python-version) myproject-env && pyenv activate myproject-env && pip install -r requirements.txt
```