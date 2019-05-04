# Neon Lines Multiplayer Game with Unity and PubNub 
![](https://2.bp.blogspot.com/-XUNcpOzrAZs/XM0eraZY1oI/AAAAAAAAxCY/jSPoGkxnBkMtUtXAB5sen77lscx3999MQCLcBGAs/s400/Hello%2BNeon%2BLines.png)

After having the chance to sit down and experiment a little bit with [Unity](https://unity.com/) and [PubNub](https://www.pubnub.com/), and seeing how easy you can use both to create engaging games or apps, I created a project named [Neon Lines](https://hielo777.github.io/NeonLines) to showcase [PubNub's Unity SDK](https://www.pubnub.com/docs/unity3d-c-sharp/pubnub-c-sharp-sdk) and how to build a fun multiplayer game.

If you have done any kind of game development, you may have heard of [Unity](https://unity.com/) . This powerful game engine allows you to create multi platform games that, with some dedication, can reach triple A level. I have always found it incredibly useful, although it may have a steep learning curve at the beginning.

[PubNub](https://www.pubnub.com/) is all about realtime applications. If you are a developer that wants to create a realtime web, mobile, or Internet of Things (IoT) applications and not having to worry about handling the complex infrastructure behind it all, I would recommend you give PubNub a good look.

The [Neon Lines](https://hielo777.github.io/NeonLines) project is a multiplayer drawing board game created with Unity, that uses PubNub's Unity SDK to distribute any player's drawing strokes to every other connected player. You can see it as drawing chat or a global graffiti wall. You can take a quick peek here:
https://hielo777.github.io/NeonLines

In this post we will go through the different aspects of creating this project and understanding the basic concepts of **PubNub** applications.
## 1. Setup
### 1.1 Unity and PubNub
I assume you already downloaded [Unity from their official page](https://unity.com/). It is free for personal use, and should take a few minutes downloading it, depending on the different features you want to include.

It is also recommended to [create your own PubNub account](https://dashboard.pubnub.com/signup). It takes just a couple of minutes and you can start checking PubNub's different features and supported platforms.

### 1.2 The project in Unity
The easiest way for you to build and run this project is to clone this GitHub's repo.

If you do this, you will have a file named Neon Lines 0519.unitypackage that you can import in unity (**Assets -> Import Package -> Custom Package**)

![](https://2.bp.blogspot.com/-oDJNVxMvMmw/XM0dryIXZsI/AAAAAAAAxCQ/3i9RRic4fQwa5NvXPJn3IsOVFUTh3Wq6QCLcBGAs/s400/importing%2Bpackage.png)

After you do this, you may see some errors appearing in Unity.
![](https://3.bp.blogspot.com/-hLoaj3_fea0/XM0ghqg6A4I/AAAAAAAAxCk/cc5zQfto3Hc3nlg_OknitxGvOyi-gZyuQCLcBGAs/s640/error%2Bpackage.png)

To solve this, enable the playmode tests for all your assemblies (Window -> General -> Test Runner)
![](https://1.bp.blogspot.com/-Gp0qFiVr54s/XM0g9NXZZRI/AAAAAAAAxCs/mHQ9DsJMXocQUijZeu8UA8L-C2-o0OvigCLcBGAs/s400/test%2Brunner.png)

And then, in the test runner window, click in the drop down menu that appear in the right corner.
![](https://1.bp.blogspot.com/-MjLslPP7t3Q/XM0homTYEiI/AAAAAAAAxC0/KVfMjf8uCDEQkGCaUdHgG62zfpQ4dHyxQCLcBGAs/s640/test%2Brunner%2Bwindow.png)

After that, you will have to restart the Unity's editor to have the changes take place.

If everything goes as planned, you should be able to see a few game objects in the sample scene.
![](https://4.bp.blogspot.com/-gkdBH-3-YhQ/XM0kzl_TrHI/AAAAAAAAxDA/1H5-ks6Tzz0HE0Hsncxiv72KapmXnfqdACLcBGAs/s320/sample%2Bscene.png)

Also, several folders and scripts in the assets folder.
![](https://4.bp.blogspot.com/-WfaznlmAdWo/XM0lAopy7TI/AAAAAAAAxDE/a-zOpi8aoj4TuipVQX5abB6tsaBDvHe3gCLcBGAs/s640/assets.png)
The NeonBoard.cs script is the most important/complex one.

You may also notice how we already have a PubNub folder that includes Unity's SDK.
![](https://3.bp.blogspot.com/-BASQiCWqOSI/XM0ll1CKfbI/AAAAAAAAxDQ/ul0pf-55FRQhSB6lgl9zxt-fSDJN9RtQQCLcBGAs/s640/pubnub%2Bfolders.png)


If you want to recreate the project from zero, it is important that you download the latest version of [PubNub's Unity SDK](https://www.pubnub.com/docs/unity3d-c-sharp/pubnub-c-sharp-sdk). You can import the package you download from PubNub the same way you can import the Neon Lines package: Going to **Assets -> Import Package -> Custom Package** and picking the right file.

Finally, you can just press play and try the game.

##Tutorial
To read a full tutorial around this project you should visit 
http://www.geekego.com/2019/05/neon-lines-multiplayer-game-with-unity.html

And don't forget to try the game here: 
https://hielo777.github.io/NeonLines
