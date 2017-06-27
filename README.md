# Backlight

Handle screen brightness on your^Wmy GNU/Linux/Emacs systems (Emacs and GNU not required, though).

## How?

Values are between 1 and 100
Any overflow/underflow will be rounded to its closest boundary (< 1 -> 1; > 100 -> 100).

4 operations:

* Get value `$ backlight`
* Set value `$ backlight 42`
* Increment value `$ backlight +10`
* Decrement value `$ backlight -10`

## Why?

Ubuntu upgrade from 16.04 to 17.04 on laptop, xbacklight broken, NIH effect, yadi yadi yada, script working on my Thinpad X260.

If not working with your environment, try to find out your `DEVICE_NAME` with the modern technology of `ls`.

Example output

```
$ ls /sys/class/backlight/
intel_backlight
```

Then edit the script, replacing the `DEVICE_NAME` variable with the value that suits your system.

## License?

```
/*
 * ----------------------------------------------------------------------------
 * "THE BEER-WARE LICENSE" (Revision 42):
 * <mota@souitom.org> wrote this file.  As long as you retain this notice you
 * can do whatever you want with this stuff. If we meet some day, and you think
 * this stuff is worth it, you can buy me a beer in return.
 * ----------------------------------------------------------------------------
 */
```

(|€~
