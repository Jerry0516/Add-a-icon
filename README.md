# Add-a-icon 加入图标
怎么做一个图标？

How to make an icon?

在Windows程序中，如果想要做一个图标，那该怎么做？

In the Windows program, if you want to make an icon, what should you do?

## 1.Make Icon 制作图标

 - 制作图标可以使用Iconlover，按[此处](https://iconlover.en.softonic.com/)下载

 - Iconlover can be used to make icons, Download [here](https://iconlover.en.softonic.com/)

 - 下载并安装好 iconlover

 - Download and install iconlover

 - 打开软件后，弹出引导对话框

 - After opening the software, the boot dialog box pops up

 - 如果你想完全自己绘制，选择【Create a new icon】

 - If you want to draw completely by yourself, select [create a new icon]

 - 如果是把已有图片转化成icon，选择【Create a new icon from image file】

 - If you want to convert an existing image to an icon, select [Create a new icon from image file]

 - 选择第二项，打开已经存在的图片

 - Select the second item to open the existing picture

 - 在图片中选择要作为 icon 的区域

 - Select the area in the picture to be the icon

 - 可以在右侧选择图标的样式，编辑好后，点击确定

 - You can select the style of the icon on the right. After editing, click OK

 - 在右侧，把不需要的图层大小删除 

 - On the right, delete the unnecessary layer size

 - 点上面的红色叉，或者按 Ctrl + Delete

 - Click the red cross above, or press Ctrl + delete

 - 通常保留48 * 48 ， 32 * 32 的就可以了。可以根据需要适当增加和减少

 - Usually keep 48 * 48, 32 * 32. Can be increased and reduced as needed

 - 注意，每个图层大小会有两个，把256色的去掉，保留32bpp的，这个像素更高

 - Note that there will be two sizes for each layer. Remove the 256 colors and keep the 32bpp one. This pixel is higher

 - 如果需要增加新的格式的图层，点击像胶卷的图标

 - If you need to add a new format layer, click the icon like film

 - 然后在弹出的对话框中选择大小和颜色

 - Then select the size and color in the pop-up dialog box

 - 图片编辑好后，点击上面的保存按钮，即可生成你想要的 icon 图标

 - After editing the picture, click the Save button above to generate the icon you want

## 2.加入图标 Add Icon
 - 新建图标资源的操作结果会写到该文件中。比如，可以通过 VC的“文件”--> “新建” --> “文件”--> “图标文件(.ico)” 来新添加一个图标，接着可以编辑该图标，最后保存。

 - The result of the new icon resource operation is written to the file. For example, you can add a new icon through VC's "file" -- > new "-- > file" -- > icon file (. ICO) ", then you can edit the icon, and finally save it.

 - 如果要添加该新建的图标，可以在文件->新建->资源脚本，如resource.rc，然后打开新建的文件，然后对着出来的resource.rc节点，右键鼠标，引入刚才的ico即可，或者插入新的ico等等，然后对着resource.rc右键鼠标选择编译，会生成一个resource.h文件，我们就可以应用这些资源了

 - If you want to add the new icon, you can use file - > New - > resource script, such as resource.rc , and then open the new file, and face the resource.rc Node, right-click the mouse, import the just ICO, or insert a new ICO and so on, and then face the resource.rc Right click and select compile to generate a resource. H file. We can apply these Resources

 - 经过上步了，现在可以用这个新建的自定义图标了，现在修改源码文件，正是使用 MAKEINTRESOURCE  这个宏来进行转换，比如：

 - 3. After the above steps, you can now use the new custom icon. Now you can modify the source file by using the makeintresource macro, for example:

 - 引入resource.h头文件

 - Introduce resource. H header file

 - wndclass.hIcon = (HICON)LoadIcon(hlnstance,MAKEINTRESOURCE(IDI_ICONAPPLICATION));

## 感谢观看 Thanks for watching
