# Git Sub-Modules Commands:

## Add the submodule(external git repo) and initializing it
```sh
git submodule add https://github.com/sriram-ponangi/dockers-k8s-demo-frontend.git submodule_dir
git submodule init
```

## Get the updated code from the upstream(original) git repo to the current submodule( update the current commit of submodule to latest)
```sh
# Change to the submodule directory
cd submodule_dir

# Checkout desired branch
git checkout master

# Update
git pull

# Go back to root directory of the project
cd ..

# Now the submodules are in the state you want, so
git commit -m "Pulled the latest version of submodule_dir"
```

## Cloning the Submodules:
```sh
# clone modules at their recorded commit when original repo is available
git submodule init 
git submodule update
```