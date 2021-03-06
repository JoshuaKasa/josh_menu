
![Rondine](https://user-images.githubusercontent.com/87675824/178853557-3705e67a-140e-40d6-8a2c-0d235d8df481.png)

# ๐งพ ***RONDINE***

Rondine is a debug menu developed for helping debugging your games in the best way possible! 
What can Rondine do?

- Check every object variable in real time.
- Modify object variables.
- Create objects.
- Copy and paste objects.
- Delete objects.
- Has a very simple GUI and setup.
- Pretty customizable.
- Works with every project.


# ๐พ **Installation**

For installing Rondine into your project you have to download the file, then open it in a GameMaker Studio 2 window and go to:

```Tools -> Create Local Package -> Name it however you want```

Once you've created the package you can go into your own project and import it by:

```Tools -> Import Local Package -> Package name```

You then succesfully imported Rondine into your project!

# ๐ช **In-game usage**

![Screenshot (495)](https://user-images.githubusercontent.com/87675824/178866714-4480bb54-bff3-4c38-9dce-cf13d9e53c35.png)

As said before, Rondine has a lot of skills, and this is how to use them all.

## Create objects
Create objects with Rondine is very easy and straight forward, you just press the **Rigth mouse button** and then select **Create** and select
your desired object.
If you have more than 10 objects in your game you'll be able to scroll down the objects list using the **Mouse wheel**.

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/87675824/178868522-b16be3f1-1362-48d1-b053-8523a6bbc1b3.gif)

## Delete objects
For deleting objects you can just press your button for opening Rondine and then select **Delete** on your selected object.

![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/87675824/178868893-daaba9b9-93d7-45dc-9712-11a3b4163e56.gif)

## Change object's variables
Changing object's variables is probably the less intuitive thing of Rondine, but once you know how to do it it's super easy!
You just select your object and then select **Variables** in the Rondine menu.
There you can see all of your object's variables (you can scroll down with the mouse wheel) and you can select one and change it 
however you want.

![ezgif com-gif-maker](https://user-images.githubusercontent.com/87675824/178868270-5687d5d8-ef36-4916-aa36-eff4f3ff707f.gif)

## Copying and pasting objects
Copying and pasting is very easy, you just select **Copy** on the object you want and then click **Paste**.
Note that the object will be created at the position of where you clicked **Paste**.

![ezgif com-gif-maker (3)](https://user-images.githubusercontent.com/87675824/178869332-842b8034-5c34-46bd-bdab-3768c9d3a21b.gif)

## Inspecting objects
Inspecting is pretty different from changing or checking object's variables.
In fact, with the inspection there's a set of pre-chosen variables that will show up on the top right, and will not be able to be changed.
For closing the inspection, either select **Back** in the Rondine menu or click on the little **X** in the top right of the inspection menu.

![ezgif com-gif-maker (4)](https://user-images.githubusercontent.com/87675824/178872278-1559b84b-ef87-4c0b-a68e-e8ea0667f5c0.gif)

# ๐ช **Usage**
Once Rondine has been imported into your project, you can place the object ***rondine_menu*** inside your room.
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
