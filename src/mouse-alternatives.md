# The Mouse; and How to Become Rat-Free

## Ergonomic Mice

I have tried several ergonomic mouse types:

- Vertical mouse
- Trackpad
- Graphical drawing pad

They all share the same problem: You have to move your hand from the keyboard to reach it.

Most of the time, I use an external trackpad as a standard mouse, e.g., for quickly positioning the cursor in a text file.

For correcting texts with Grammarly, I use a 13.3" Pen Tablet (Wacom One).

## Keyboard Mouse

On a QMK-driven keyboard, you can enable keys for mouse movements and clicks in the file `rules.mk`:

```
MOUSEKEY_ENABLE = yes
```

In the `keymap.c`, the mouse keys are defined by `KC_MS_UP` (move cursor up), `KC_MS_DOWN` (move cursor down), `KC_MS_BTN1` (press button 1), etc. As well, pointer speed, acceleration, and other parameters can be finely tuned.

Therefore, the mouse can be replaced by keyboard actions to a large extent.

## Encoders

Encoders can replace typical mouse actions, such as scrolling. For example, you can define a left encoder for left/right, and a right encoder for up/down scrolling. In addition, you can define actions for pressing the encoder buttons. In combination with a keyboard-friendly browser, you can therefore navigate the web with little mouse use.
