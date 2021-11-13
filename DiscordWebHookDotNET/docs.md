## DiscordWebHookDotNET

## About

DWDN was something I made just for the hell of it, its a very standard C# WebHook wrapper for Discord, and it's meant to be modified.

I know its very bad, thats why you modify it

## Code 

You can find the whole source code here: https://github.com/swiney-2/DiscordWebHook.NET

# Settings

Note: You NEED to set these in Settings.cs before doing anything further

```csharp
/// <Settings>
/// Stuff you need to set before using any other stuff eee
/// </Settings>
        <Uri> WebHookURL; //The URL of the webhook
        <string> Message; //The message the WebHook it will send
        <string> Username; //The username of the WebHook
        <Uri> ProfilePicture; //The profile picture of the WebHook
```
```csharp
 <void> SendMessage()
 //Sends a message, all of the contents are set in Settings.cs
```
```csharp
  <void> DeleteWebHookAsync()
  //Deletes Settings.WebHookURL;
```

```csharp
 <bool> Exists()
 //Returns true if the WebHook exists, otherwise returns false
```
