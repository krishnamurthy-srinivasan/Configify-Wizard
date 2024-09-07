# Configify Wizard

`Configify Wizard` is a Python package designed for managing and converting configuration files. It supports parsing configurations from YAML, CFG, and CONF files, and provides functionality to write configurations to `.env` files, JSON files, or set them as environment variables.

## Features

- **Read Configuration Files**: Supports YAML, CFG, and CONF file formats.
- **Write Configuration**: Save configurations to `.env` or JSON files.
- **Set Environment Variables**: Easily set configurations as environment variables.

## Installation

You can install `Configify Wizard` via pip:

`bash
pip install Configify-Wizard

## Usage

Here’s a quick guide to using Configify Wizard:

### 1. Parse Configuration Files
You can read configuration files in YAML, CFG, or CONF formats:

`inline code`

```python
from config_parser_module import ConfigParserModule

config_parser = ConfigParserModule()

# Read YAML file
config_dict = config_parser.read_yaml('config.yaml')

# Read CFG or CONF file
config_dict = config_parser.read_cfg('config.cfg')

```
### 2. Write Configurations

You can write configurations to a .env file or a JSON file:

`inline code`

```python
# Write to .env file
config_parser.write_env('./config.env')

# Write to JSON file
config_parser.write_json('./config.json')

```

## 3. Set Environment Variables

`inline code`
```python
config_parser.set_os_env()
```