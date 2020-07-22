# Hello

---

##  step 1 สร้างไฟล์ Workflow ใน Project

```sh
$ mkdir <project>/.github/workflows
$ touch main.yml
```

## ในไฟล์ main.yml

```yaml
name: CI
on:
  push:
    branches: [ master ]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v2
    - name: Run a one-line script
      run: pwd
```

# Push Event

```sh
$ git add -A
$ git commit -m 'demo git action'
$ git push origin master 
```

---

เพิ่มเติม -> [ทำ Github Action แบบเร็วๆ](https://blog.jaedsada.me/github-action/)
