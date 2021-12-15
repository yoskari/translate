# Translate
## Concept
This is just a simple python script that first checks a local csv file for translations and examples.
If the translations aren't found locally, the script uses the LibreTranslate API to get a translation.
Getting the translations locally is faster and can give you better translations and examples with the word.
However offline dictionaries/wordlists can be lacking in usually don't have conjugated words, this is where
machine translation is useful because it always gives you something.

## Dependencies
libretranslatepy

## Installation
clone the repo
```bash
git clone https://github.com/yoskari/translate.git && cd translate
```

install dependencies
```bash
pip3 install -r requirements.txt
```

make the script into an executable
```bash
chmod +x translate
```

## Use
### interactive mode (Russian to English only)
```bash
./translate
```
### run with arguments
the first argument is the word or sentence you want to translate
The optional second argument is the language code (en, ru, es etc.), which defaults to auto

Autodetect language:
```bash
./translate привет
```
Translate a word from a specific language
```bash
./translate hola es
```
Translate a sentence from a specific language
```bash
./translate "Как дела?" ru
```

# Links
[Google spreadsheet for the words](https://docs.google.com/spreadsheets/d/1hSsPR0fN7I456-TZOUFJwOb7GjSrqeoOo02hMCy9NfI/edit#gid=7)

[LibreTranslate](https://github.com/LibreTranslate/LibreTranslate)
