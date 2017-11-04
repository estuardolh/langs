git
---
  init a empty repo
  ```
  git init
  ```

  add a remote origin to a empty repo
  ```
  git remote add origin <url here>
  ```

  push and merge local changes to Remote
  ```
  git push -u origin master
  ```
  where -u references to 'upstream'

  example of update a local repository from "origin" link from remote repository
  ```
  git pull [origin master]
  ```

  set credentials
  ```
  git config --global user.name "username"
  git config --global user.email "mail"
  ```
  get credentials
  ```
  git config user.name
  git config user.email
  ```
