![demo](~kubelive.gif)

<div style="text-align: center">
  <a target="_blank" rel="noopener noreferrer" class="no-decoration" href="https://npm-stat.com/charts.html?package=kubelive&from=2015-01-01&to=2019-12-31">
    <img class="html-image" src="https://img.shields.io/npm/dy/kubelive.svg?style=for-the-badge" alt="npm-downloads">
  </a>
  <a target="_blank" rel="noopener noreferrer" class="no-decoration" href="https://www.npmjs.com/package/react-lazyload">
    <img class="html-image" src="https://img.shields.io/github/stars/ameerthehacker/kubelive.svg?style=for-the-badge" alt="github-stars">
  </a>
</div>

## Tech Stack <i class="fas fa-layer-group"></i>

<i class="fab fa-react react"></i> React

## Motivation

I felt that the output from **kubectl get pod -w** is very cluttered and it is a pain in my ass to understand which pod is running, which pod is exactly terminating so I built **kubelive** which updates the status of the pods in realtime without cluttering the terminal

## Installation

Make sure you have node installed and then run the command

```sh
npm install -g kubelive
```

## Available commands

- List the pods in the clutser

```sh
kubelive get pods
```

- List the services in the clutser

```sh
kubelive get services
```

- List the replication controllers in the clutser

```sh
kubelive get replicationcontrollers
```

- List the nodes in the clutser

```sh
kubelive get nodes
```

- List the pods in the cluster in a jiffy

```sh
kubelive
```