# :t-rex: GamepadZilla la la!

> A plug-and-play gamepad frontend framework for HTML5 mobile games, supporting both virtual and physical joysticks. _No scripting required._

### :joystick: Features

 * gpz is fast. _(no DOM manpulation)_
 * gpz is easy. _(no Javascript needed, use only html5 attributes)_
 * gpz is pure. _(made with only typescript without dependencies)_
 * gpz hates the van's old-man! <!-- punkzilla reference -->

### :video_game: Preview

![virtual gamepad](https://raw.githubusercontent.com/RodrigoDornelles/RodrigoDornelles/master/media/gamepadzilla-1-0-1.gif)

## :minibus: How to use

 * import library with [npm](https://www.npmjs.com/package/gamepadzilla) or [cdn](https://www.jsdelivr.com/package/npm/gamepadzilla)
 * create html5 **canvas** elements with class `gpz-joy` or `gpz-btn` and configure data attributes.

```html
<!DOCTYPE html>
<html>
    <head>
        <script src='https://cdn.jsdelivr.net/npm/gamepadzilla@1/dist/gamepadzilla.js'></script>
    </head>
    <body style="touch-action: none">
        <canvas
            class="gpz-joy"
            data-gpz-bind="ArrowUp ArrowLeft ArrowDown ArrowRight">
        </canvas>
        <canvas
            class="gpz-btn"
            data-gpz-bind="KeyF">
        </canvas>
    </body>
</html>
```