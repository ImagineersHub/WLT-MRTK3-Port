# WLT-MRTK3-Port

We have been using this port for months with MRTK3, Unity 2021 and Unity 2022. It primarily provides support for using AR Foundation's XROrigin and related changes.

This port is not actively supported by FuzzyDoorTech

Missing 'FrozenWorld' namespace
Errors like the following (usually a lot):

Assets\WorldLocking.Engine\Plugin.cs(10,37): error CS0234: The type or namespace name 'FrozenWorld' does not exist in the namespace 'Microsoft.MixedReality' (are you missing an assembly reference?)

It is missing the FrozenWorld.Engine DLL. See NuGet Setup.

Using NuGet For Unity
Make sure the nuget.org feed is in sources. Check this in Unity > Edit > Preferences > NuGet for Unity. If not, either:

Use the Add New Source GUI in Unity > Edit > Preferences > NuGet For Unity to add the same share.

Replace "New Source" with a name of your choosing (for example, "NuGet").
Replace "source_path" with "http://www.nuget.org/api/v2/".
After confirming the nuget.org feed, in Unity > NuGet > Manage NuGet Packages, find and install the latest version of Microsoft.MixedReality.FrozenWorld.Engine. (Search for "FrozenWorld".)

To update to a later version, open the Unity > NuGet > Manage NuGet Packages again, and find the FrozenWorld.Engine package and select Update. Note: You may have to the Updates tab to find the version you are looking for.
