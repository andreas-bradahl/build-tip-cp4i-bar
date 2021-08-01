# build-tip-cp4i-bar
CLI application to create an overridden BAR articact file for IBM App Connect Enterprise

## Usage
The folder structure of your TIP CP4I application needs to be the following:
```
{git-repo-name}
    projects
        {application-1}
        {application-2}
        ...
        {application-n}
    config
        {environment-1}
            baroverides
                {git-repo-name}.{environment-1}.properties
        {environment-2}
            baroverides
                {git-repo-name}.{environment-2}.properties
        ...
        {environment-n}
            baroverides
                {git-repo-name}.{environment-n}.properties
```

The subfolders in the `config` folder needs to have a BAR override file with name **{git-repo-name}.{environment}.properties** in the folder called `baroverides`

1. Navigate to the root folder (the one represented by the git-repo-name above) of your TIP CP4I application
2. Run script with the environment as a parameter, for instance:
```
python build_bar.py qa
```
3. An overridden BAR file should now be placed in your `baroverides` folder
