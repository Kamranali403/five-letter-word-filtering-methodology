# Five-Letter Word Filtering Methodology

This repository explains a simple methodology for filtering five-letter words using letter positions, included letters, excluded letters and known patterns.

The methodology can be used for word-game tools, educational projects, linguistic analysis and puzzle-solving applications.

## Purpose

Searching a complete word list manually can be slow. A structured filtering process reduces the list by applying several conditions in a logical order.

The main filtering conditions are:

* Word length
* Starting letters
* Ending letters
* Included letters
* Excluded letters
* Correct letter positions
* Included but misplaced letters
* Known patterns

## Basic filtering process

### 1. Confirm word length

Only entries containing exactly five alphabetic letters should remain in the dataset.

### 2. Apply known positions

If a letter is known to occupy a specific position, keep only words containing that letter in the required position.

For example, the pattern `C _ A _ E` requires:

* `C` in position 1
* `A` in position 3
* `E` in position 5

### 3. Apply included letters

An included letter must appear somewhere in the word. If its position is known to be incorrect, words placing it in that excluded position should also be removed.

### 4. Remove excluded letters

Words containing confirmed excluded letters should be removed from the results.

### 5. Apply starting and ending filters

Starting and ending filters can further narrow the results when the beginning or ending of the word is known.

## Example

Consider the following conditions:

* Five letters
* Pattern: `C _ A _ E`
* Must include: `R`
* Must not include: `S`

A filtering system checks the word list against every condition and returns matching possibilities such as `CRANE` and `CRATE`.

## Possible applications

This methodology can support:

* Five-letter word finders
* Word-game solving tools
* Crossword assistance
* Vocabulary exercises
* Letter-frequency research
* Educational word projects

## Interactive implementation

Readers who prefer to apply these filters without writing code can use the [interactive five-letter word finder on WordHubPro](https://wordhubpro.com/).

WordHubPro combines starting, ending, included, excluded and position-based filters with a Wordle-style solver and word unscrambler.

## Future additions

Planned additions to this repository include:

* A small properly licensed sample dataset
* Letter-frequency tables
* Position-based frequency analysis
* Simplified filtering examples
* Additional methodology documentation

## Licence

The original material in this repository is available under the MIT License. Any third-party dataset added in the future must retain its original licence and attribution requirements.

## Contributions

Suggestions and corrections are welcome through GitHub Issues.
