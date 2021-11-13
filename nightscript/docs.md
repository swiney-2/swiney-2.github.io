## Nightscript Documentation

## About

Nightscript is a project I made for fun, I was bored a couple months ago and wanted to try to recreate Lua in C#, which eventually changed into making my own language, which eventually changed into making a language base to customize.

## Code 

You can find the whole source code here: https://github.com/swiney-2/Nightscript

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

## NS_FILE_SYS


``` csharp
 <string> FILESYS_READFILE(<string> Path)
 //Returns the raw text of a file located at <string> Path
```


``` csharp
 <bool> FILESYS_FILE_EXISTS(<string> DirectoryPath)
 //Returns the true or false value of a file existing at <string> DirectoryPath
```


``` csharp
 <void> DIRECTORY_DEL(<string> Path)
 //Deletes directory at <string> Path
```


``` csharp
<void> FILESYS_APPEND_TEXT(<string> Path, <string> Data)
//Appends the text <string> Data to file located at <string> Path
```


``` csharp
<void> DIRECTORY_NEW(<string> Path)
//Creates a directory at <string> Path
```


``` csharp
<void> FILE_WRITE(<string> Path, <string> Data)
//Writes text <string> Data at file <string> Path
```


``` csharp
<void> FILE_NEW(<string> path)
//Creates a new file at <string> Path
```


``` csharp
<void> FILE_DELETE(<string> FilePath)
//Deletes file located at <string> FilePath
```


``` csharp
<bool> RETURN_FILE_EXISTS(<string> FilePath)
//Returns a boolean value of a file existing at <string> FilePath
```

## NS_HTTP

Http client

```csharp
 <string> LOAD_STRING_URL(<Uri> Url)
 //Returns the content of <Uri>
```
```csharp
<enum> HTTP_REQ_TYPE { 
          GET,
          DELETE,
        }
        //The supported Http methods, add/remove as you like
```
```csharp
 HTTP_REQ(<Uri> Url, <HTTP_REQ_TYPE> Method)
 //Sends Http request <HTTP_REQ_TYPE> to <Uri>
```

## NS_MESSAGEBOX


```csharp
<enum> NS_MESSAGEBOX_BUTTON
        {
            TXTALRT_OK,
            TXTALRT_OKCANCEL,
            TXTALRT_YESNO,
            TXTALRT_YESNOCANCEL,
            TXTALRT_ABORT_RETRY_IGNORE,
            TXTALRT_RETRY_CANCEL,
        }
        //The different types of MessageBoxButtons
```
```csharp
 <enum> NS_MESSAGEBOX_ICON
        { 
         TXTALRT_NONE,
         TXTALRT_HAND,
            TXTALRT_QUESTION,
            TXTALRT_EXLAMATION,
            TXTALRT_ASTERISK,
            TXTALRT_STOP,
            TXTALRT_WARNING,
            TXTALRT_ERROR,
            TXTALRT_INFORMATION,
        }
        //The different types of MessageBoxIcons
```
```csharp
 <void> NEW(<string> text, <string> label, <NS_MESSAGEBOX_BUTTON> button) {
```
