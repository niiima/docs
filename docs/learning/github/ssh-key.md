###List Existing keys :

`ls -al ~/.ssh`

If there is none generate one:

Paste the text below, substituting in your GitHub email address.

`$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`

It save it in `C:\Users\home\.ssh`
Copy it to clipboard and past in the section inside git account setting.

###Add the SSH key to your GitHub account.

## Test it 
`λ ssh -T git@github.com`


## Change https to git

` λ git remote set-url origin git@github.com:psybient/webpack-migration.git`