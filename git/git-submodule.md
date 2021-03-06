# Git Submodule

## Clone

with all submodules

```shell
git clone --recurse-submodules [remote_origin]
```

## Commands

- add
- update
- foreach
- summary
- deinit
- init

## Usage

### Add Submodule

### Update Submodule

Update to remote version

```shell
git submodule update --remote
```

```shell
git submodule update --remote --recursive
```

Update to local commit version

```shell
git submodule update
```

### Foreach Submodule

```shell
git submodule foreach git log --oneline
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

### Init

```shell
git submodule init app
```
