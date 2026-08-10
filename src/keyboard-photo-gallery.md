# Keyboard Photo Gallery

This is a sample gallery chapter. The old repository contains 79 keyboard photos (222MB total) in the `keyboard-photos/` directory.

## Strategy for Integrating Photos

Given the large number of photos, I recommend:

1. **Select the best photos**: Choose 10-20 representative photos that best illustrate different keyboard types, builds, and use cases.

2. **Organize by theme**: Group photos into categories like:
   - Split keyboards
   - Dactyl Manuform builds
   - Travel keyboards
   - Workspace setups
   - Building process

3. **Create a dedicated chapter**: Add a "Keyboard Gallery" chapter to showcase the photos.

4. **Use subdirectories**: Organize photos in subdirectories within `src/figures/`:
   ```
   src/figures/keyboard-photos/
   ├── split-keyboards/
   ├── dactyl-manuform/
   ├── travel-setups/
   └── building-process/
   ```

5. **Optimize images**: Resize large photos to appropriate web resolution (e.g., 1000-1500px wide) to reduce file size.

## Example Photo References

Once photos are organized, you can reference them like:

```markdown
![Corne keyboard build](figures/keyboard-photos/split-keyboards/corne-build.jpg)

![Dactyl Manuform workspace](figures/keyboard-photos/workspace/dactyl-setup.jpg)
```

## Current Photos in Old Repository

The `../Keyboards-Book/keyboard-photos/` directory contains:
- 79 JPG/PNG photos
- Total size: 222MB
- Dates range from 2020-2022
- Includes builds, workspaces, and construction photos

Would you like me to:
1. Copy all keyboard photos to the new repository?
2. Select and copy only the best 10-20 photos?
3. Create the gallery chapter structure?
4. Leave them in the old repository for now and add a note about their availability?
