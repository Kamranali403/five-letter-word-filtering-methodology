# Five-Letter Word Filtering Methodology

This documentation explains the methodology behind filtering five-letter words using known positions, required letters, excluded letters, patterns, and repeated-letter rules.

The goal is to turn puzzle clues into clear filtering conditions that reduce a large word list to a smaller group of useful candidates.

## What This Documentation Covers

- Filtering by correct letter positions
- Including known letters in unknown positions
- Excluding invalid letters
- Handling repeated letters correctly
- Combining multiple conditions
- Testing filters with practical examples

## Purpose of the Project

This project documents the filtering principles used by the [WordHubPro five-letter word finder](https://wordhubpro.com/). The documentation focuses on the underlying method so that developers, puzzle players, and researchers can understand how candidate words are selected.

## Basic Filtering Process

A five-letter word list can be filtered in the following order:

1. Keep words that match all known letter positions.
2. Remove words containing excluded letters.
3. Keep words containing every required letter.
4. Check whether repeated letters are allowed or required.
5. Review the remaining words as possible solutions.

## Documentation Sections

Continue with the Filtering Method section for a detailed explanation of each filtering condition. The Repeated Letters section covers one of the most commonly misunderstood parts of five-letter word filtering.
