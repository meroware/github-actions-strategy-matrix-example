# Github Actions Strategy Matrix Examples
mike

> Provides examples on different ways to use strategy matrix in github actions

[![Strategy Matrix Walkthrough](https://img.youtube.com/vi/z_fjpPbaAgw/0.jpg)](https://www.youtube.com/watch?v=z_fjpPbaAgw)

> Click To Watch ☝️ - The Matrix of Github Actions

![Matrix run Diagram](./assets/matrix-run-diagram.png)

## Workflow Examples
```
.github
└── workflows
    ├── sample-matrix-do-not-exit-early.yml
    ├── sample-matrix-exit-early.yml
    ├── sample-matrix-max-parallel.yml
    ├── sample-matrix-use-includes-json-syntax.yml
    ├── sample-matrix-use-includes-syntax.yml
    └── sample-matrix.yml
```


- sample-matrix.yml
    - Shows simple matrix usage by providing fixed values
    
        ![Sample Matrix Parallel](https://github.com/meroware/github-actions-strategy-matrix-example/workflows/Sample%20Matrix%20Parallel/badge.svg)

- sample-matrix-max-parallel
    - Shows how to add max number of parallel jobs in the matrix to allow running at the same time
    
        ![Sample Run Max 2 Jobs In Parallel](https://github.com/meroware/github-actions-strategy-matrix-example/workflows/Sample%20Run%20Max%202%20Jobs%20In%20Parallel/badge.svg)
    
- sample-matrix-exit-early
    - Shows how if one job fails within the matrix the whole matrix of jobs will fail
    
        ![Sample Should Fail All Runs](https://github.com/meroware/github-actions-strategy-matrix-example/workflows/Sample%20Should%20Fail%20All%20Runs/badge.svg)

- sample-matrix-do-not-exit-early
    - Shows how to let the strategy know not to exit the matrix if one of the jobs withing the matrix fails
    
        ![Sample Should Fail Run 1 Only](https://github.com/meroware/github-actions-strategy-matrix-example/workflows/Sample%20Should%20Fail%20Run%201%20Only/badge.svg)

- sample-matrix-use-include-syntax
    - Shows include syntax in yaml format
    
        ![Sample Run Include Syntax](https://github.com/meroware/github-actions-strategy-matrix-example/workflows/Sample%20Run%20Include%20Syntax/badge.svg)

- sample-matrix-use-include-json-syntax
    - Shows include syntax in json format
    
        ![Sample Run Include Syntax Json Format](https://github.com/meroware/github-actions-strategy-matrix-example/workflows/Sample%20Run%20Include%20Syntax%20Json%20Format/badge.svg)
