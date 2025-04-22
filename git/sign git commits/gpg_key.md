## install gnupg
sudo pacman -S gnupg

## find your git config email
git config --global --list

## generate new gpg key
gpg --full-generate-key
### choose (1) RSA and RSA
### set key size to 4096 for security
### set expiration date
### enter your GitHub email when prompted
### set a paraphrase

## find your gpg key id
gpg --list-secret-keys --keyid-format=long
### key id is the text after "rsa4096/"

## export your public key
gpg --armor --export <gpg_key_id>
### add this key to GitHub -> Settings -> SSH and GPG keys -> New GPG Key

## configure Git to use the gpg key
git config --global user.signingkey <gpg_key_id>
git config --global commit.gpgsign true
