#plog
Portable and simple log for C++

#Inroduction

##Features
* Very small
* Easy to use
* Headers only
* Cross-platform
* Thread and type safe
* No 3rd-party dependencies
* Skip execution if log is disabled
* Txt and Csv formatters
* Automatically log `this` pointer (supported only on Visual Studio)

#Usage

##Include
1. Add `plog/inlcude` to the project include paths
2. Add `#include <plog/Log.h>` into your cpp/h files (if you have procompiled headers it is a good place to add this include there)

##Initialization

```cpp
plog::init("log.csv", plog::debug, 1000 * 1000, 5);
```

##Logging

```cpp
LOG_ERROR << "error";
```

#Competing C++ log libraries
* [Boost::Log](http://www.boost.org/doc/libs/release/libs/log/)
* [EasyLogging++](https://github.com/easylogging/easyloggingpp)
* [g2log](http://www.codeproject.com/Articles/288827/g-log-An-efficient-asynchronous-logger-using-Cplus)
* [glog](https://code.google.com/p/google-glog/)
* [Log4cplus](http://sourceforge.net/projects/log4cplus/)
* [Log4cpp](http://log4cpp.sourceforge.net/)
* [Log4cxx](http://logging.apache.org/log4cxx/)
