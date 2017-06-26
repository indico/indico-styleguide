<p align="center">
  <img src="https://github.com/indico/indico/blob/master/indico/htdocs/images/logo_indico.png" width="300">
</p>

# Indico Styleguide

This is the styleguide of the [Indico project](https://github.com/indico/indico). Here you'll find useful components to help you develop Indico's UI solutions. This guide contains real working examples, code snippets, documentation, and style guidelines. The styleguide is build on top of [Fabricator](https://github.com/fbrctr/fabricator).

## Installing styleguide
Clone repo:
```
git clone --recursive git@github.com:indico/indico-styleguide.git
```

With the indico virtualenv active, initialize Indico’s submodules:
```
cd indico-styleguide/indico
fab setup_deps
```
From the project’s root directory, start the server:
```
npm start
```

## Updating styleguide
Commit the changes in the master branch:
```
git add src/materials/components/buttons/10-button.html
git commit -m “Add i-button documentation”
git push upstream master
```
Generate output code and deploy on gh-pages:
```
gulp default # Generates output code
gulp deploy  # Pushes code to the gh-pages branch
```

## Fetching Indico style changes
Since Indico is a submodule of the styleguide project, the only necessary thing to do in order to fetch the latest Indico code is to update the submodule:
```
cd indico
git pull
cd ..
git add indico
git commit -m “Update Indico submodule”
```

## Resources
* http://fbrctr.github.io (Fabricator documentation)
* https://goo.gl/aBPTt7 (Deploying To Github Pages With Gulp)
* https://goo.gl/FLwmBz (Indico presentation)



