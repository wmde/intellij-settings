# IntelliJ settings

Settings for IntelliJ based IDEs, currently only a WMDE code style.

## Using the settings

This repository mirrors the structure of the IntelliJ settings directory.

To use all or some settings from this repository, copy the needed files from this repo to your
IDEs settings directory. Conversely, to add new settings to this project, copy them from your
IDEs settings directory to the corresponding place in this git repo.

Example location of the settings directory on Kubuntu:

    ~/.PhpStorm2017.2/config
    
You can find the directory via the IDE itself by opening File -> Import Settings, which should
select the settings directory. (The import/export functionality does not work with this git repo.)

## WMDE code style

This is the code style used at WMDE, originally based on the MediaWiki code style, though with
some additions, primarily for recent versions of PHP.

The goal of the configuration in this repository is that you can use the "Reformat Code" IDE
action without it breaking the formatting already there. This allows you to not immediately fix
spacing issues and the like while you are writing code, and instead just hit the appropriate
hotkey after finishing your line(s).

The goal is explicitly not to pin down everything that can be possibly pinned down. There are
differences between developers and teams that do not contradict the WMDE code style, and where
possible, the configuration in this repository should not interfere with those differences.
Due to the way the IDE works, sometimes it is however needed to pick one particular approach
over another, due to the lack of an "allow both" option in the configuration. If you want to
have a more strict version with your own preferences, please create a new CS config file.
