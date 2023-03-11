# MW-EZCV

This is a slightly modified version of the original [ezcv](https://github.com/Descent098/ezcv).

## Changes

Minor changes were made from the original ezcv.

Notably, the `dimension` theme has been altered slightly to:
* Remove the messsages in Experience and Projects section saying "Below are my ...".
* The LinkedIn link in the About section now properly links to LinkedIn, rather than Instagram.
* The active cards now appear slightly transparent.
* The border colours have been changed from White to Pink.
* Scrollbars have been removed.

## Usage

MW-EZCV is only effective when using the dimension theme.

1. To use this modified version of ezcv, you would need to build, install, and replace your current version of ezcv; from version `0.3.x` to `MW-0.3.x`.

2. To uninstall your current ezcv installation, run: ` pip uninstall ezcv ` and accept any prompts.

3. To replace it, clone this repository and run `setup.py build` and then `setup.py install`. You should have 2 new folders: `build/` and `dist/`.

4. Go to your repository that contains your website's contents, and ensure that running `ezcv -v` returns `MW-0.3.x` (where x is your version number, `7`).
    * If you don't see `MW-x.x.x`, you did not uninstall the orignal ezcv properly. Navigate to ezcv's installation location and remove it there and ensure your terminal cannot find any instance of ezcv before retrying step 3.

5. Ensure `ezcv -p` previews as normal.

6. Run `ezcv theme dimension -c`. This should copy the dimension theme into your repository, so that ezcv can use the modified dimension theme, rather than the default.

7. Push to GitHub.