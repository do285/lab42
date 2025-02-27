# Lab Objectives

1. [OWASP Dependency Check](https://github.com/jeremylong/DependencyCheck) scan must be run on each opened pull request
2. Push all successfully checked pull requests to main branch
3. [OWASP Dependency Check](https://github.com/jeremylong/DependencyCheck) scan must be run on each push to main branch
4. Project must use NPM or YARN

# Lab Documentation

[OWASP-prepared action for SCA on GitHub](https://github.com/dependency-check/Dependency-Check_Action) and [GitHub Action for approving pull requests](https://github.com/juliangruber/approve-pull-request-action) has been used.

Repository file (.github/workflows/push_main.yml) performs scans on each push to main branch.

Repository file (.github/workflows/pull_open.yml) performs scans on each opened pull request and if it succeeds it accepts it - GitHub then should automatically merge the code.

# Todo App

A simple buggy todo app

# Installation
```bash
git clone https://github.com/qxb3/todo-app.git
cd todo-app
npm install #or yarn
```

# Running
```bash
# Running development
npm run dev

# Building
nom run build
```
