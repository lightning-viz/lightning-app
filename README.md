Lightning app
-------------
Extra assets for bundling lightning as a standalone app. To bundle (for OS X), first clone the lightning repo, then install and build

```
npm install
npm run electron-rebuild
``` 

Install electron-packager and run it on the resulting folder 

```
electron-packager lightning Lightning --platform=darwin --arch=x64 /
  --version=0.30.1 --icon=lightning/electron/icons.icns --prune /
  --app-version=0.1.13 --app-bundle-id=Lightning --helper-bundle-id=Lightning
```

Unzip ``tempolate.dmb.bzip2`` and mount ``template.dmg``. Drag the app we just built into the disk image (in the appropriate position on the well on the left!), select it inside Disk Utility, and select Images -> Convert. That's it!
