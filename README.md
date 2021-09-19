# app_theme
Submodule to generate a unique app theme across all flutter apps.
By setting the ThemeData of a MaterialApp, a consistent look is achieved.
## How to install
This repository is meant to be a included as a submodule of flutter apps.
Just navigate to your `lib` directory and add the submodule where you would like. E.g.
```
cd lib
cd util
git submodule add https://github.com/flognity/app_theme.git
git submodule init
git submodule update
```
Simply include the ThemeData in your MaterialApp Constructor call:
```
AppTheme appTheme = AppTheme();

MaterialApp(
      theme: appTheme.getTheme(isDarkTheme: false),
      darkTheme: appTheme.getTheme(isDarkTheme: true),
      //...
    );
```
## License
MIT License

Copyright (c) 2021 flognity
