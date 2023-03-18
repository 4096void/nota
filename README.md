## General
- RSA
  - generate, `ssh-keygen -t ed25519 -C "4096void@gmail.com"`
  - copy, `pbcopy < ~/.ssh/id_ed25519.pub`
- Readline
  - previous(next) one in history, ctrl + p(n)
  - move, ctrl + a(|<-), alt + b(<<), ctrl + b(<), ctrl + f(>), alt + f(>>) ctrl + e(->|)
  - delete, ctrl + u(to beginning), ctrl + w(one word before), alt + d(one word after), ctrl + k(to end)

## GR
- moved, if dest dir doesn't exists, `mv -vn from_dir/**.JPG to_dir`
- renamed end with `_1`, `find . -depth -name "*.JPG" -exec sh -c 'f="{}"; mv -- "$f" "${f%.JPG}_1.JPG"' \;`

## Git
- delete branch in local & remote, `git branch -d ${local_branch} && git push orogin -d ${remote_branch}`
- create branch in local & remote, `git checkout -b <branch> && git push -u origin <branch>`
- revert last commit in local & remote, `git reset --hard head~1 && git push -f origin`
