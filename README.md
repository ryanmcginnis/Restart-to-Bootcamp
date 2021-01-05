**Note:** Not actively maintained, but updated by community contribution as of December 2020.

# Restart to Bootcamp

- Uses Automator to reboot system to Bootcamp. 
- Made under macOS Sierra 10.12.2.  
- Tested under macOS Catalina 10.15.7 with TouchID bypass.
- Updated for macOS Big Sur 11.0.1, and used CliClick (<https://www.bluem.net/en/projects/cliclick/>) as a dependency because AppleScript's ability to mouse-click is abysmal.

## Install as Finder Service

1. From a shell (Terminal) window, execute `brew install cliclick` (note: if you need Homebrew installed go to <https://brew.sh/>)
1. Download "Restart to Bootcamp" workflow file.
1. Right-click the file. Click _Open with... -> Automator_.
1. Change `thePWD` to your adminstrator password (also edit `theCLI` if needed). Save the workflow.
1. Right-click file again. Click _Open with... -> _Automater Installer_.

**Ready to test:**  You can now select "Restart to Bootcamp" from the _Finder > Services..._ menu.  If you don't see it, check _System Preferences > Keyboard > Shortcuts > Services > General_ (check "Restart to Bootcamp")

### Optional Enhancement

You can also add it to the Touchbar from _System Preferences > Keyboard > Customize Control Strip..._ and ensure Quick Actions is in your bar.

## Alternate: Install as an Application

1. Do Steps 1-3 in the Install as a Finder Service
1. From within Automator, click _File --> Convert to..._ and save as an Application.
1. Place the saved Application inside your Applications folder (or wherever you want) and you can double-click it or pin to your Dock for easy access.

##

**Note:** Allow Finder to control the system from _System Preferences > Security & Privacy > Accessibilty > Privacy_

## After the jump...

You can optional download the "Quit System Preferences" workflow Application and set this to run at login under _System Preferences > Users & Groups > Login Items_ (for your user account).  This will close the System Preferences panel left open from the Restart to Bootcamp operation when you come back into macOS.  You can load the Application in Automator to verify it just executes that single action.
