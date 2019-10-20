# TFUtil

A simple script that will help you create Terraform file structure

## Requirments

- Python 3.6+

## Command line options

```
    -i, --init           -- creates root file structure
    -i, --add-module     -- creates module's directory with files
    -e, --add-env        -- creates directory for environment
```

Default file structure:

*ROOT_FILE_TEMPLATE_LIST:*
```
 main.tf, provider.tf, backend.tf, vars.tf, outputs.tf, README.md
```

*MODULE_FILE_TEMPLATE_LIST:*
```
main.tf, vars.tf, outputs.tf, README.md
```

*MODULES_FOLDER:* is `modules`

*ENV_FILE_TEMPLATE_LIST:*
```
main.tf, vars.tf, outputs.tf, README.md
```

### Profiles

You can create different profiles in config file [.tfutil_profile.ini](.tfutil_profile.ini) and specify that profile in cmd

```
--profile=my_profile
```

## Installation

- Download this repo:
```
    git clone https://github.com/dmakeienko/tfutil.git ~/.tfutil
```

- Add ~/.tfutil to your $PATH:
```
    echo 'export PATH="$HOME/.tfutil:$PATH"' >> ~/.bash_profile
```

## License
See file [LICENSE](LICENSE)
