<div style="text-align: center;">
    <img src="/assets/images/logo.png" width="400">
</div>

# Al Ehsaan Website

- Production website (`Main` Branch): [https://www.al-ehsaan.org](https://www.al-ehsaan.org)


## 1. Jekyll

> We are using Jekyll framework for the website. This section notes how to use Jekyll and the directory stucture used for development.


### 1.1. Install Ruby & Jekyll (Quick Start)

The easiest way to install Ruby and Jekyll is by using the [RubyInstaller](https://rubyinstaller.org/) for Windows.

RubyInstaller is a self-contained Windows-based installer that includes the Ruby language, an execution environment, important documentation, and more.

This guide only covers the installation of RubyInstaller-2.4 and newer here.

1. Download and install a **Ruby+Devkit** version from [RubyInstaller Downloads](https://rubyinstaller.org/downloads/). Use default options for installation.
2. Run the `ridk install` step on the last stage of the installation wizard. This is needed for installing gems with native extensions. You can find additional information regarding this in the [RubyInstaller Documentation](https://github.com/oneclick/rubyinstaller2#using-the-installer-on-a-target-system). From the options choose `MSYS2 and MINGW development tool chain`.
3. Open a new command prompt window from the start menu, so that changes to the `PATH` environment variable becomes effective. Install Jekyll and Bundler using the following command:
```bash
gem install jekyll bundler
```
4. Check if Jekyll has been installed properly: 
```bash
jekyll -v
```


### 1.2. Detailed Jekyll Documentation

[Read Jekyll documentation](https://jekyllrb.com/)

### 1.3. Folder Structure:

```
|--- assets
|    |--- css                     : Cascading Style Sheets
|    |--- images                  : Images
|    |--- js                      : Javascripts
|    \--- pdf                     : Documents
|
|--- _data
|    |--- top-navigation.yml      : Manages Top Navigation Menu
|    \--- class-robotics-2022.yml : Example of photo and video file with type used in _posts
|--- _includes
|--- _layouts
|--- _plugins
|--- _posts
\--- .github
     |--- config
     |--- ISSUE_TEMPLATE
     \--- workflows
```


## 2. Github

### 2.1. Clone Code Repository

```
git clone https://github.com/zalam003/al-ehsaan.git
cd al-ehsaan
```


### 2.2. Running Jekyll Webserver Locally

```bash
jekyll build
jekyll serve
```


### 2.3. Github Naming Convention & Process

- Create new brach from `main`
- Naming convention for branch: issueNumber-devInitial-shortDescriptionOfIssue
- Push changes to new feature branch
- Open Pull Request (PR)
- Post PR for review
- Once approved Merge to `main` branch
- Open `merge issueNumber-devInitial-shortDescriptionOfIssue into main` PR
- Merge PR
