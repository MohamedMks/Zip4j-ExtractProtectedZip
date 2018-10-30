# Zip4j-ExtractProtectedZip

This is a gradle version of Zip4j old library (from http://www.lingala.net/zip4j/ )

How to add to your project 
 - add this to your project level gradle file.
 ---
 maven { url 'https://jitpack.io' }
 ---
 - add this to your module dependencies
 ---
 implementation 'org.bitbucket.MohamedMks:zip4j-extractprotectedzip:-SNAPSHOT'
 ---



How to use this library
```
 try {
    ZipFile zipFilee = new ZipFile("ZIP_FILE_LOCATION");
    if (zipFilee.isEncrypted()) {
        zipFilee.setPassword("ZIP_PASSWORD");
    }
    zipFilee.extractAll(unzipLocation);

} catch (ZipException e) {
                    
}
```

