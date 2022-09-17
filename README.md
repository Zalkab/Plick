# Plick
**Plick is a small and lightweight game engine created by Zalkab**, which is intented for simple games. It is very easy and intuitive, and will also be updated constantly.

If you have any questions, feel free to message me on Discord: zalcab#1371

## Specifications
* Runs with Windows [System.Drawing](https://docs.microsoft.com/en-us/dotnet/api/system.drawing?view=net-6.0) (I know it is quite scuffed but I was lazy using Open GL)
* Built in C# in a .NET Framework
* Uses [Box2DNet](https://github.com/codeyu/Box2DNet) to handle physics
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
```
## Adding Shapes
You can easily add rectangles into the squares using the Shapes2D function. You will then have to add the paremeters for the position, scale and tag of the object. Here is an example of a square.
```cs
Shape 2D player = new Shape2D(new Vector2(10, 10), new Vector2(10, 10), "Test");
```
## Adding Sprites
Adding sprite its not to hard either. You can use the Sprite2D function which needs a position, scale, root of the Sprite and a tag of the Sprite. Be aware that all the images must be inside a folder called `Assets` which must be located inside `bin/Debug`. Note the engine only accepts .png and the extension is not needed in the root parameter.
```cs
Sprite2D player = new Sprite2D(new Vector2(10, 10), new Vector2(36, 45), "Sprites/Players/player1", "Player");
```
## Creating levels
There are probably lots of different ways of creating levels
