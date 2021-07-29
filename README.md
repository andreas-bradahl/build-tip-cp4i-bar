# build-tip-cp4i-bar
CLI application to create an overridden BAR articact file

## Usage
The folder structure of your TIP CP4I application needs to be the following:
```
<git-repo-name>
    projects
    config
        local
        readyapi
        test
        qa
        prod
```

The subfolders in the `config` folder needs to have a BAR override file with name **<git-repo-name>.<environment>.properties** in the folder called `baroverides`

1. Navigate to the root folder (the one represented by the git-repo-name above) of your TIP CP4I application
2. Run script with the environment as a parameter, for instance:
```
python build_bar.py qa
```