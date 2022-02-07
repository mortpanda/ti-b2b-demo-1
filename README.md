# angular-b2b-demo-1

# THIS IS NOT AN OFFICIAL TEMPLATE.  
This is was created for personal projects.

# What does this application do?
- This application obtains a list of apps assigned to the Okta user, and displays them as a dashboard item,
- The application uses the org authorisation server, so the issuer URL needs to be the org URL,
- The user account to demo this app, needs to be a super admin on the org.

# Required scopes
- openid
- email
- profile
- address
- okta.users.read.self
- okta.apps.read
- okta.groups.manage

# Configuration file
- Needs to be placed in `/src/app/shared/okta` as  `okta-config.service.ts`, with the below variables,
  ```
  strBaseURI = '{{ Base URL }}';
  strRedirectURL = '{{redirect URL}}';
  strClientID = '{{ Client ID }}';
  strIssuer = '{{ Issue URL, which must be the org URL }}';
  strPostLogoutURL = '{{ Post logout URL }}';
  strScope = ['openid', 'email', 'profile', 'address','okta.users.read.self','okta.apps.read','okta.groups.manage'];
  strResponseType = 'code';
  strResponseMode = 'fragment';
  strPrompt = 'consent';
  strPkce = true;
  strLang = '{{ language }}';
  strBrand = '{{ Brand color in HEX }}';
  strLogo = "assets/img/okta-japan-logo.jpg";
  ```

# How to display your apps on the dashboard
- If an app is to be displayed on the dashboard, prefix the app with `b2b_enabled_Angular - ` .


## Development Environment
```
    / \   _ __   __ _ _   _| | __ _ _ __     / ___| |   |_ _|
   / △ \ | '_ \ / _` | | | | |/ _` | '__|   | |   | |    | |
  / ___ \| | | | (_| | |_| | | (_| | |      | |___| |___ | |
 /_/   \_\_| |_|\__, |\__,_|_|\__,_|_|       \____|_____|___|
                |___/


Angular CLI: 11.0.4
Node: 14.15.0
OS: linux x64

Angular: 11.0.4
... animations, cli, common, compiler, compiler-cli, core, forms
... language-service, platform-browser, platform-browser-dynamic
... router
Ivy Workspace: Yes

Package                         Version
---------------------------------------------------------
@angular-devkit/architect       0.1100.4
@angular-devkit/build-angular   0.1100.4
@angular-devkit/core            11.0.4
@angular-devkit/schematics      11.0.4
@angular/cdk                    11.2.13
@angular/flex-layout            12.0.0-beta.34
@angular/http                   7.2.16
@angular/localize               11.2.14
@angular/material               11.2.13
@schematics/angular             11.0.4
@schematics/update              0.1100.4
rxjs                            6.6.3
typescript                      4.0.3


```

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.


## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Screenshots
<img src="/Capture.PNG" alt="drawing" width="600"/>
<img src="/Capture2.PNG" alt="drawing" width="600"/>
<img src="/Capture3.PNG" alt="drawing" width="600"/>
<img src="/Capture4.PNG" alt="drawing" width="600"/>

