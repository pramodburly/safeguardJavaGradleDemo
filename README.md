# safeguardJavaGradleDemo

Example to download SafeGuard artifact through Gradle build 

* prefer 'latest.release'  

```
Could not resolve com.oneidentity.safeguard:safeguardjava:{prefer latest.release}.
     Required by:
         project :
      > Could not resolve com.oneidentity.safeguard:safeguardjava:6.11.0.133386.
         > inconsistent module metadata found. Descriptor: com.oneidentity.safeguard:safeguardjava:6.11.0 Errors: bad version: expected='6.11.0.133386' found='6.11.0'

```

* require 'latest.release'
```
 Could not resolve com.oneidentity.safeguard:safeguardjava:latest.release.
     Required by:
         project :
      > Could not resolve com.oneidentity.safeguard:safeguardjava:6.11.0.133386.
         > inconsistent module metadata found. Descriptor: com.oneidentity.safeguard:safeguardjava:6.11.0 Errors: bad version: expected='6.11.0.133386' found='6.11.0'

```

* require '[6.11['
```
Could not find com.oneidentity.safeguard:safeguardjava:[6.11[.
     Required by:
         project :
```

* require '6.11['
```
 Could not find com.oneidentity.safeguard:safeguardjava:6.11[.
     Required by:
         project :

```

* strictly '6.11['
```
 Could not find com.oneidentity.safeguard:safeguardjava:6.11[.
     Required by:
         project :

```