# Readme

```mermaid
flowchart LR
    id0((start)) --> Build
    Build --> Deploy
    Deploy --> id00((End))
    subgraph Build
        direction TB
        id1[Setup] --> id2[Render]
        id2 --> id3[Publish] 
        id3 --> id4[Commit]
        id4 --> id5[Push]
    end
    subgraph Deploy
        direction TB
        id6[Setup] --> id7[Deploy to github pages]
    end

```


# Important

You need to enable an option in the project settings to make this work.

[here](https://www.raulmelo.me/en/til/how-to-solve-permission-to-x-denied-to-github-actions-bot#:~:text=Permission%20to%20%22x%22%20denied%20to,option%20Read%20and%20write%20permissions.)