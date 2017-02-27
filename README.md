# Set Xcode Git Build Number
![Team](https://img.shields.io/badge/team-silver-lightgray.svg)
![Status](https://img.shields.io/badge/status-active-green.svg)

This is a Bitrise step to aid in CI. This step will generate a build number based off the current date and latests git commit. The build number for the app and all extensions will be updated to the new generated build number.

## How to use this Step 

Int the bitrise.yml file for your workflow add this step before xcode-archive
```
- git::https://github.com/InVisionApp/steps-set-xcode-git-build-number.git@master: {}
````
    
## How to test

1. Download [Bitrises CLI tool](http://devcenter.bitrise.io/docs/bitrise-command-line-interface-how-to-guide).
2. Clone this repo
3. Create a file in the new repo named ".bitrise.secrets.yml"
4. Add the line
    MY_PLIST_PATHS : <directory to Xcode project>
5. Run `bitrise run test`
