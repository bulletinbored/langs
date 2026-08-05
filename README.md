# bulletinbored-langs

Translation files for [bulletinbored](https://github.com/yourusername/bulletinbored), a minimal PHP forum.

## Structure

Each translation is a single PHP file in the repository root:

```
en.php
it.php
de.php
fr.php
```

The filename must match the language code (e.g. `en`, `it`, `de`, `fr`).

## File Format

Every file must return an associative array with `key => translated string`:

```php
<?php
return [
    'site_name' => 'bulletinbored',
    'home' => 'Home',
    'login' => 'Login',
];
```

Use the English keys exactly as they appear in the core `lang/en.php` file. Missing keys will fall back to English.

## Adding a New Language

1. Fork this repository.
2. Create a new file named `<language_code>.php` in the root directory.
3. Translate every key from `en.php`.
4. Open a pull request with the new file.

## For Forum Administrators

You can install language files directly from the Admin Panel:

1. Go to **Admin Panel → Languages**.
2. Use the **Install from GitHub** section to browse available translations.
3. Click **Install** next to a language to download it to your forum.

You can also manually upload a `.php` translation file from the same page.
