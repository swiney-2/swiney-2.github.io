## NS_STACK

A stack/console library

``` csharp
 <void> NS_CLEAR_OPT()
 
 //Clears the console/output
```

``` csharp
 <void> CHAR_COUT_NL(<string> Text)
 
 //Writes string Text to the console/output
```

``` csharp
 <void> CIN()
 3
 //Prompts a character input
```

``` csharp
 <void> DBG_COUT(<string> Text)
 
 //Writes string Text to the debug console
```


``` csharp

 <void> COUT(<string> Text)
 //Prompts character output of string Text
```


``` csharp
 <void> FOREGROUND_SET(<ConsoleColor> color)
 //Sets the console foreground to ConsoleColor color
```

## NS_CRYPT

A crypt library

``` csharp
 <string> HASH_SHA256(<string> RawData)
 
 //Returns a Hashed string of RawData
```
NS_CRYPT.BASE64
``` csharp
 <string> ENCODE_NEW(<string> Data)
 
 //Returns a Base64 encoded string of Data
```

``` csharp
<string> DECODE_NEW(<string> Data)

//Returns a decoded string of a Base64 encoded string

```
