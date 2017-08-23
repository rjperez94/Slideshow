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
