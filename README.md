# springlobby flatpak package

Additional steps might be required to get flatpak working see 
https://docs.flatpak.org/en/latest/first-build.html

## Build 

```
flatpak-builder --force-clean build-dir com.springrts.springlobby.yaml
```

## Test

```
flatpak-builder --run build-dir com.springrts.springlobby.yaml springlobby
```

## Install

```
flatpak-builder --install --user --force-clean build-dir com.springrts.springlobby.yaml
```

Run installed version:
```
flatpak run com.springrts.springlobby
```