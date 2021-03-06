# Transliterator #

A PHP < 5.4 fallback for `transliterator_transliterate()`

For original version, use:
> composer require lukemadhanga/php-transliterator

This version:
> set it as a repositories package in composer.json

PHP 5.4 has a built-in function, `transliterator_transliterate()` which does exactly what it says on the tin. This class works as a basic fallback for that function which is available from PHP5.4 with the `intl` package installed.

#### Supported Blocks ####

    Basic Latin
    Latin-1 Supplement
    Latin Extended-A
    Latin Extended-B
    IPA Extensions Block
    Spacing Modifier Letters
    Combining Diacritical Marks
    Greek and Coptic
    Cyrillic
    Cyrillic Supplement
    Armenian
    Georgian
    Latin Extended Additional
    Greek Extended
    General Punctuation
    Superscripts and Subscripts
    Combining Diacritical Marks for Symbols
    Georgian Supplement
    Cyrillic Extended-A
    Cyrillic Extended-B
    Latin Extended-D
    
#### This version (added) ####
    Arabic

#### Usage (this version) ####

    # If no composer:
    include_once 'path/to/Transliterator.php';
    
    echo \Voult\Transliterator::convert('Antonín Dvořák'); // Antonin Dvorak
