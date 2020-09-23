# Licence-Secret-File-Generator
This is sub project which is writtent in C#, inorder generate sercret encrypted file , where developer can keep
cutomizable filds with valuse such as licence key, expiry date etc 

## Classes
The project utilizing Package class for creating the package and  two classes for Creating and Encrypting files namely,
1. Binary SerialiZation 
2. Serialize Helper
# Methods 
You can use ``Serialize and Deserialize`` methods to create and open files.
# How to Read file information in C#.
Include the c# classes in your projects and Deserialize the file as follows 
```
 var plist = SerializeHelper.DeserialilZe<ObservableCollection<PackageClass>>(licenceFile.lic);
                    var version = (from p in plist.AsEnumerable() where p.PName == "VERSION" select p.Pvalue).ElementAt(0);
```

