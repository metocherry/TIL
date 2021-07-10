# Git Submodule

## Commands

- add
- deinit

## Usage

### Add Submodule

### Delete Submodule

#### 1. deinit

```shell
# git submodule dinit -f <directory>
git submodule deinit -f test_app
```

#### 2. delete .git/modules

```shell
rm -rf .git/modules/test_app
```

#### 3. delete the folder

```shell
git rm -f test_app
```
