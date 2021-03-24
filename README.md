`en_US` dictionary files are downloaded by following [hunspell's official document](https://github.com/hunspell/hunspell#usage).

```
wget -O en_US.aff 'https://cgit.freedesktop.org/libreoffice/dictionaries/plain/en/en_US.aff?id=a4473e06b56bfe35187e302754f6baaa8d75e54f'
wget -O en_US.dic 'https://cgit.freedesktop.org/libreoffice/dictionaries/plain/en/en_US.dic?id=a4473e06b56bfe35187e302754f6baaa8d75e54f'
```

# `hunspell` without personal dictionary

```
~/ghq/github.com/kyanny/test-hunspell-dic main*
❯ hunspell -d en_US -l test.txt
kyanny.
```

# `hunspell` with personal dictionary

```
~/ghq/github.com/kyanny/test-hunspell-dic main*
❯ hunspell -d en_US -p my.dic -l test.txt
JavaScript.
hunspell(31530,0x116e88dc0) malloc: *** error for object 0x7ff49a805e80: pointer being freed was not allocated
hunspell(31530,0x116e88dc0) malloc: *** set a breakpoint in malloc_error_break to debug
zsh: abort      hunspell -d en_US -p my.dic -l test.txt
```

# IntelliJ IDEA Ultimate spellcheck without personal dictionary

![idea-without-personal-dictionary.png](./idea-without-personal-dictionary.png)

# IntelliJ IDEA Ultimate spellcheck with personal dictionary

![idea-with-personal-dictionary.png](./idea-with-personal-dictionary.png)
