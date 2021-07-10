# Git Submodule

## Commands

- add
- update
- summary
- deinit

## Usage

### Add Submodule

### Update Submodule

Update to remote version

```shell
git submodule update --remote
```

Update to local commit version

```shell
git submodule update
```

### Delete Submodule

#### 1. deinit

```shell
# git submodule dinit -f <directory>
git submodule deinit -f app
```

#### 2. delete .git/modules

```shell
rm -rf .git/modules/app
```

#### 3. delete the folder

```shell
git rm -f app
```
