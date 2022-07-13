
![Rondine](https://user-images.githubusercontent.com/87675824/178853557-3705e67a-140e-40d6-8a2c-0d235d8df481.png)

# Documentation

Rondine is a debug menu developed for helping debugging your games in the best way possible!

## Installation

For installing rondine into your project you have to download the file, then open it in a GameMaker Studio 2 window and go to:

```Tools -> Create Local Package -> Name it however you want```

Once you've created the package you can go into your own project and import it by:

```Tools -> Import Local Package -> Package name```

You then succesfully imported Rondine into your project!

## Usage
Once Rondine is inside your project, you can place the object ***rondine_menu*** inside your room.
Note that Rondine is a persisent object and so it will exists in every room after you place it inside one.
Note also that you could have GUI size problems, since Rondinde resizes when it's created (you can always change it inside your code).

## Modify aesthethic
Rondine is a versatile tool that can be modified however you want.
First off, the aesthethic... You can change the Rondine's aesthethic by going into:

```Rondine -> Functions -> rondine_menu_settings```

There you can find all of the Rondine's options, especially colors.

## Add options
As said before, Rondine is very versatile, in fact, you can add various options and make them function as you want.
For adding an option you wanna go to:

```Rondine -> Objects -> rondine_menu -> Create Event```

Once in the create event you wanna go into the **options** array, and for adding a new option you want to:

![carbon](https://user-images.githubusercontent.com/87675824/178851638-0165cb94-1e26-4bdd-b8e6-4e123434404d.png)

This would be an example option:

![carbon (1)](https://user-images.githubusercontent.com/87675824/178851856-66fa8097-1ef0-4529-913a-e5ae8187f39e.png)


## Excluding certain objects
Rondine gives you the possibility of excluding certain objects that you don't want to inspect or debug.
For doing that you wanna go to:

```Rondine -> rondine_menu -> Go to the last line -> excluded_objects[] -> Object name + .id```

This is an example:

![carbon (2)](https://user-images.githubusercontent.com/87675824/178852721-542c84bb-72d3-42d2-8dbd-bd36b0f424c4.png)

Here I'm excluding the objects: **oPlayer, oCamera, oMouse** (remember that you must put ``.id`` at the end of each object name for this to work). 