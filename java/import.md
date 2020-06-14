# Java

## Import

General syntax:

```java
// import package
import packagename;

// import specific class
import packagename.MyClass;

// import specific class from subpackage
import packagename.subpackagename.MySubClass;

// import everything from "packagename"
import packagename.*;
```

A same package can be imported only once.

`import` must be top-level, otherwise a compilation errors occurs.

To import a single class, `import` statements must specify the fully qualified name of that class (i.e. respect the hierarchy declared by that class' `package` statement).