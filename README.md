# Morse <-> Text

Simple script to translate from text to morse code and backwards.

Morse code consists of the characters ```−``` (for a long signal) and ```·``` (for a short signal).

## Usage

### Cli

```
λ py morse_code.py -h
usage: morse_code.py [-h] input

Translate between morse code and plain text

positional arguments:
  input       either plain text or morse code

optional arguments:
  -h, --help  show this help message and exit
```

### Module

```python
import morse_code as morse

print(morse.translate(STRING_TEXT))

```
Where ```STRING_TEXT``` is a text string (i.e. ```'test'```) either of morse code or text.

## API

### translate()

Input: String (i.e. ```test how``` or ```− · ··· −    ···· −−− ·−−```)

Output: String (i.e. ```− · ··· −    ···· −−− ·−−``` or ```test how```)

Takes a string as parameter and returns the translated input as string.