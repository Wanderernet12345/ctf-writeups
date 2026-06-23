# Bandit Level 2 → 3

## Objective
Find the password stored in a file called --spaces in this filename--, 
located in the home directory.

## Challenge
The filename was `--spaces in this filename--`. Two problems here:
- Spaces in filename break normal `cat` usage
- Filename starts with `--` which Linux interprets as a flag/option

## Commands Used
```bash
ssh -p 2220 bandit2@bandit.labs.overthewire.org
ls
cat -- --spaces\ in\ this\ filename--
```

## Why This Works
- `--` tells the command "no flags after this" — 
  so Linux stops treating `--spaces` as a command option
- Quotes around the filename handle the spaces inside it

## What I Learned
- Filenames starting with `-` or `--` need special handling using `--`
  before the filename
- Filenames with spaces must be wrapped in quotes or spaces 
  escaped with backslash `\ `
- Both problems can exist in the same filename simultaneously

## Screenshot
![Level 2 to 3](../../screenshots/bandit/level-02-03.png)
