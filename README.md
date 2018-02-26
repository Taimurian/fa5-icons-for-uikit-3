Font Awesome 5 for UIKit-3 Framework
====

**UIkit's icon library can be extended and customized with your own icon files.**

You can easily add Font Awesome 5 Icons to [UIKit framework][4] by including them in UIkit's build process with the following steps

#### 1- Setup UIkit from [Github source][1]
#### 2- Download The optimized Font Awesome 5 icons from this repo.
#### 3- Include your prefered SVG icons in UIkit's build process.

Copy your prefered icons to your desired icons folder. The build process will check 3 places for svg icon files:
* The Source folder: ```/src/images/icons/*.svg```
* The custom folder: ``` /custom/icons/*.svg```
* Any custom theme: ```/custom/mytheme/icons/*.svg ```

#### 4- Compile UIkit to include all your icons.
```
npm run compile
```
Your additional icons will now be added to the icon library, in one of these two places:
* ```dist/js/uikit-icons.js``` if you have added the icon to UIkit globally
* ```dist/js/uikit-icons-mytheme.js``` if the icon is only inside a UIkit theme

Make sure to include the icon library script, for more details see the [installation instructions][2].

#### 5- Usage

Add your icons anywhere in your content in the same way you [add icons in UIKit 3][3].

Please notice that I have prefixed all the icons with ```fa-``` to prevent conflict with any existing icons.

```html
// Basic Example 

<span uk-icon="fa-chrome"></span> 
```
```html
// With Ratio 

<span uk-icon="icon: fa-bitcoin; ratio: 3.5;"></span>

```
```html
// Ass Buttons 

<a href="#" class="uk-icon-button" uk-icon="fa-twitter"></a>
```

**[Demo][5]**

### License
The original Font Awesome 5 icons created by Dave Gandy can be found at [http://fontawesome.io][6]
UIKit 3 Framework [License][7]


**Enjoy :)**

[1]: https://github.com/uikit/uikit
[2]: https://getuikit.com/docs/installation
[3]: https://getuikit.com/docs/icon
[4]: https://getuikit.com
[5]: https://taimurian.github.io/fa-icons-for-uikit3/
[6]: https://fontawesome.com/
[7]: https://github.com/uikit/uikit/blob/develop/LICENSE.md

