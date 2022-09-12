# Plick
**Plick is a small and powerfull game engine created by Zalkab**, which is intented for simple games. It is very easy and lightweight, and will also be updated constantly.

If you have any questions, feel free to message me on Discord: zalcab#1371

## Specifications
* Runs with Windows [System.Drawing](https://docs.microsoft.com/en-us/dotnet/api/system.drawing?view=net-6.0) (I know it is quite scuffed but I was lazy using Open GL)
* Built in C# in a .NET Framework
*
## Installation Guide
1. Create a new [.NET 4 Framework Console Application](https://www.youtube.com/watch?v=sAWHLUpxCJI)
2. 
# Doc
## Destroying objects
To destroy objects you can use the method `DestroySelf`. Be aware that this will only remove then from the list, so they will technically still exist, leading to more memory usage. To completly remove the object set the object `= null`.
```cs
if(object != null) 
{
  object.DestroySelf();
  object = null;
}
## Adding Shapes
You can easily add rectangles into the squares using the Shapes2D function. You will then have to add the paremeters for the position, scale and tag of the object. Here is an example of a square.
```cs
player = new Shape2D(new Vector2(10, 10), new Vector2(10, 10), "Test");
