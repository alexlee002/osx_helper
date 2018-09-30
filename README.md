# osx_helper

A shell script to customize backup your docs/apps/settings and restore them in your new Mac OS.

## When I need it

* when you reinstall your OS ...
* when you have a new mechine ... 
* Anytime you decide to do.

## Usage

### backup:

Customize backup your files, settings(defaults) to the backup path. 

* edit `files` phase in `osx_helper.json` to specify which files to backup.
* edit `defaults` phase  to specify which domains of defaults to backup.

    ```bash
    osx_helper backup /path/to/backup
    ```
### restore

* install homebrew
* Optimize you system: edit `osx_config` phase  in `osx_helper.json` to config it.
* restore the files from specified backup path,  you can specify which files/defaults to be restored via editing `osx_helper.json`.
* install apps via homebrew,  which configured in `brews` phase.
* install and config `oh-my-zsh` 

```
osx_helper restore /path/to/prev_backup
```

### init

The same as restore action,  exclude the step 2（restore files and defaults）.

```
osx_helper init
```

