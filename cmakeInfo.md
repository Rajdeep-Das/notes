## CMake helpful stuff

CMake comes with numerous modules that aid in finding various well-known libraries and packages. You can get a listing of which modules your version of CMake supports by typing cmake --help-module-list, or by figuring out where your modules-path is and looking inside of it. On Ubuntu linux, for example, the module path is /usr/share/cmake/Modules/

Command-line:
```sh
cmake --help-module-list
cmake --help-module FindGTest
```

You can write new modules using: pkg-config
Example command:
```sh
pkg-config --libs /usr/local/Cellar/sqlite/3.8.8.3/lib/pkgconfig/sqlite3.pc
```

### Sources
- http://www.cmake.org/Wiki/CMake:How_To_Find_Libraries
- http://people.freedesktop.org/~dbn/pkg-config-guide.html