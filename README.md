# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for Pip.WebUI 2

This is a workspace for [Pip.WebUI2](https://github.com/pip-webui2/pip-webui2) HTML5 framework for LoB applications.
It enables build, test, and release across the following projects.

Components:
- **Layouts** - Responsive application layouts
- **Nav** - Navigation controls
- **Behaviors** - Attachable behaviors
- **Themes** - Color themes support
- **Controls** - Basic controls
- **Buttons** - Various buttons
- **Cache** - Caching behavior
- **Landing** - Controls for landing pages
- **Locations** - Location controls
- **Pictures** - Picture controls
- **Documents** - Document controls
- **Files** - File upload controls
- **Dates** - Date and time controls
- **Composite** - Composite content controls
- **Dialogs** - General-purpose dialogs
- **Errors** - Error controls and pages
- **Entry** - Entry pages
- **Shell** - Application shell components

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone git@github.com:pip-webui2/pip-webui2-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop infrastructure services
```bash
> piptask start -component pip-webui2-nav
> piptask stop -component pip-webui2-nav
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

