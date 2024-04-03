## Step by step i18n setup in Astro project

### 1. Change site header and integrate a language picker

- Create `i18n` folder to contains files related to this feature.
- `ui.ts` and `utils.ts` in `i18n` folder are responsible to handle translations and manipulate url to include language folder in the link.
- Move menu links passed as prop of Header.astro from `navigation.js` to `Header.astro` and `Footer.astro` then there will be no need of that `navigation.js` file because we need to use window object to get the URL and that is impossible in `navigation.js` since `.astro` called server side.  
- Created a `LanguagePicker.astro` to offer a dropdown list with the right paths.

### Create website page for a new language.

- Under `pages` folder created `ar` folder where includes all pages copied from the same folder `pages`.
- Change layout to include the language `<html lang={lang}..` which I find not managed yet by the onwidget Github account behind the theme.

### Create website blog post for a new language.

- Copied all posts under `content/post/` to `content/post/ar`.
