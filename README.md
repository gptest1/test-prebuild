# test-prebuild

```yml
# .gitpod.yml
tasks:
  - name: Install dependencies
    before: |
      echo `gp url` >> before.txt
      npm install
      gp sync-done install
    command: |
      echo `gp url` >> command.txt
      gp sync-await install
      npm start

github:
  prebuilds:
    master: true
    branches: true
    pullRequests: true
    pullRequestsFromForks: false
    addCheck: true
    addComment: false
    addBadge: false
```

touch  
touch  
touch 20
