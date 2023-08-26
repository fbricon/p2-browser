## Features

* Browse contents of p2 repository as a list or grouped by features
* Filter view by installable feature id or provided capabilities
* See composite repositories structure
* Save repository metadata and individual artifacts locally
* See installable unit dependency tree and list (try it, highly recommended!)
* See installable unit direct and indirect references
* See features that include installable unit

## Building and running p2-browser locally

To build and run p2-browser as a standalone RCP application:

* Make sure a JDK 17 or more recent is installed and available on PATH
* Clone this git repository locally
* From base directory of the clone run the following command

```
    ./mvnw clean package
```


* RCP applications for all enabled platforms will be created under the directory:

```
com.ifedorenko.p2browser.rcp/target/products/com.ifedorenko.p2browser.rcp/
```

  Both packed and unpacked versions are created

```
    ├── com.ifedorenko.p2browser.rcp
    │   ├── linux
    │   │   └── gtk
    │   │       └── x86_64
    │   ├── macosx
    │   │   └── cocoa
    │   │       └── x86_64
    │   └── win32
    │       └── win32
    │           └── x86_64
    ├── com.ifedorenko.p2browser.rcp-linux.gtk.x86_64.tar.gz
    ├── com.ifedorenko.p2browser.rcp-macosx.cocoa.x86_64.tar.gz
    └── com.ifedorenko.p2browser.rcp-win32.win32.x86_64.zip
```

* To start p2-browser, execute p2browser (or p2browser.exe, on Windows) from the root of the RCP app
  for your platform.
