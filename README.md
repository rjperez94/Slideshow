# Slideshow

## Compiling Java files using Eclipse IDE

1. Download this repository as ZIP
2. Create new `Java Project` in `Eclipse`
3. Right click on your `Java Project` --> `Import`
4. Choose `General` --> `Archive File`
5. Put directory where you downloaded ZIP in `From archive file`
6. Put `ProjectName/src` in `Into folder`
7. Click `Finish`
8. Move all the images in the `images` directory from `{ProjectName}/src` to the root of your `Java Project` i.e. `{ProjectName}`

### Linking the UI Library

9. Right click on your `Java Project` --> `Build Path` --> `Add External Archives`
10. Select `ecs100.jar` and link it to the project. That JAR will be in the directory where you downloaded ZIP

## Running the program

1. Right click on your `Java Project` --> `Run As` --> `Java Application` --> `SlideshowApp`

## Build an executable using IntelliJ IDEA

1. Go to **File** → **Project Structure** → **Artifacts**.
2. Click the green plus (**+**) button, select **JAR**, and choose **From modules with dependencies...**
3. In the **Main Class** field, click the folder icon and select the application's entry point class.
4. Under **JAR files from libraries**, select **extract to the target JAR** (this creates the single Fat JAR).
5. Click **OK**, then click **Apply**.
6. From the top menu bar, go to **Build** → **Build Artifacts...** and click **Build**.
7. The executable jar file will be generated inside the project directory under `out/artifacts/`.

### Run the executable JAR file using the command line:

```bash
java -jar path/to/executable.jar
```

## Live Demo

You can run this application directly in your web browser via the link below:

**[Launch Live Demo](https://rjperez94.github.io/Slideshow/)**

### Loading Local Data

If you are trying to pick a file from your physical hard drive, you cannot browse your local folders through the Java window. You must use the bridge upload feature.

1. Look at the very top right of the Java window's title bar for a small **Up Arrow (Upload)** button.
2. Click it to trigger your **native browser file picker** (this one can see your real computer folders).
3. Select your local file. The app will silently drop it into the virtual folder named `/files/uploads/`.
4. Now, inside your Java file picker, type `/files/uploads/` into the file path bar and press **Enter** to find your uploaded file.


## Notes

You may use the left and right cursor keys to navigate, if the image pane has the focus.

## Modes

<strong>Click appropriate mode to switch between the two modes</strong>

### Creator Mode

- Add random image before `current` image, initialise if none
- Add random image after `current` image, initialise if none
- Remove `current` image, if any
- Remove all images, if any
- Select image to the left of `current` image. You can use `left arrow key` too
- Select image to the right of `current` image. You can use `right arrow key` too
- Select image at the end
- Select image at the start
- Reverse image ordering

### Viewer Mode

- View images using `left` and `right` arrow keys
- Slide show (interval 2 seconds)
