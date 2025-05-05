# Patches

### How to create a patch
```
cd blockball
git diff > plugin.primary.patch
```
### How to apply a patch 

```
git apply BlockBallCommandExecutor.ArenaCreation.patch
```

### Update submodule.

```
git submodule foreach git pull origin master
```
