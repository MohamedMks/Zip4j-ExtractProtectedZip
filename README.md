# Zip4j-ExtractProtectedZip

[![N|Solid](https://scontent-mrs1-1.xx.fbcdn.net/v/t1.0-1/c10.0.40.40a/p40x40/27657539_2074458639504608_7695734048125776429_n.jpg?_nc_cat=106&_nc_ht=scontent-mrs1-1.xx&oh=e9dbaaaedf05ffdeeb1262ccbbc6eece&oe=5C734A6E)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://bitbucket.org/MohamedMks/zip4j-extractprotectedzip)

This is a gradle version of Zip4j old library (from http://www.lingala.net/zip4j/ ) .
  - unZip protected zip files 

# How to add to your project  !

  - add this to your project level gradle file.
```sh
    maven { url 'https://jitpack.io' } 
```
  - add this to your module dependencies.
```sh
     implementation 'org.bitbucket.MohamedMks:zip4j-extractprotectedzip:-SNAPSHOT'
```

# How to use this library  !
```sh
 try {
    ZipFile zipFilee = new ZipFile("ZIP_FILE_LOCATION");
    if (zipFilee.isEncrypted()) {
        zipFilee.setPassword("ZIP_PASSWORD");
    }
    zipFilee.extractAll("UN-ZIPED_FILES_LOCATION");
} catch (ZipException e) {
                    
}
```


### Plugins

No need for any .

| Plugin | Link |
| ------ | ------ |
| Name | url |

### Todos

 - Encryption 

License
----

Free For ALL


**Free Software, Hell Yeah!**


