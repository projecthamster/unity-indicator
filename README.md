# Hamster Indicator

Hamster Indicator is an interface for [Project Hamster](http://projecthamster.wordpress.com/), a time-tracking application. It adds an application indicator to the panel in Unity, Ubuntu's default desktop environment.

**This is meant to work with Hamster as it is in the trunk, not with the latest stable version. It is still a work in progress and not ready for proper installation**

(If, however, you want to test it, just run hamster-indicator. The icon won't be properly displayed. The entry "Indicator Options" on the menu isn't implemented yet. The windows may not always come to the front. Other than that, it should work, if you have installed Hamster from the trunk. [Tell us about any bugs](https://github.com/projecthamster/unity-indicator/issues). See also [issue #184](https://github.com/projecthamster/hamster/issues/184).)

## Features

![Example screenshot](https://cloud.githubusercontent.com/assets/904912/5063658/79376efc-6def-11e4-9b72-6540db6780a3.png)

## Installation


- dependencies
  - Hamster 2.0-rc1
- get the source
```sh
git clone https://github.com/projecthamster/unity-indicator.git```
```
- install
```sh
cd unity-indicator
sudo cp data/hamster-indicator.gschema.xml /usr/share/glib-2.0/schemas/
sudo glib-compile-schemas /usr/share/glib-2.0/schemas
sudo cp data/icons/ubuntu-mono-dark/24x24/* /usr/share/icons/ubuntu-mono-dark/apps/24/
sudo gtk-update-icon-cache /usr/share/icons/ubuntu-mono-dark
sudo cp hamster-indicator /usr/local/bin/hamster-indicator
```

- Starting

`hamster-indicator`


## Contributing

1. [Fork](https://github.com/projecthamster/unity-indicator/fork) this project
2. Create a topic branch - `git checkout -b my_branch`
3. Push to your branch - `git push origin my_branch`
4. Submit a [Pull Request](https://github.com/projecthamster/unity-indicator/pulls) with your branch
5. That's it!
