Django Tutorial Translation
---------------------------

1. Get django tutorial sources and extract translatable messages into .pot files:

        $ make gettext

2. Setup/Update your locale_dir (for spanish, for example):

        $ sphinx-intl update -p _build/locale -l es

3. Translate your .po files under ./locale/<lang>/LC_MESSAGES/.

4. Build .mo files and make translated document.

        $ sphinx-intl build
        $ make -e SPHINXOPTS="-D language='es'" html
