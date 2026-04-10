# PicoCTF — Git Challenge Writeup

## Challenge Name
Git Impersonation

## What the Challenge Said
Push flag.txt as user root with email root@picoctf to get the flag.

## What I Did

1. Cloned the repository using git clone
2. Read the README — understood I needed to push as a specific user
3. First attempt — pushed as wrong user — server rejected it
4. Realised git config controls who you appear to be
5. Changed name to root and email to root@picoctf
6. Pushed flag.txt again — server accepted it
7. Got the flag

## What I Learned

Git does not verify identity. Anyone can commit as anyone 
by changing git config user.name and user.email. 
Real systems use GPG-signed commits to prevent this.

## Flag
picoCTF{1mp3rs0n4t4_g17_345y_367122f4}

## Date
[April 10,2026]
