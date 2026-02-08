# git_mastery_with_ssk

# 📦 Git Areas & Command Flow

This diagram shows the four main areas created when you clone a Git
repository and how common commands move changes between them.

------------------------------------------------------------------------

## 🗂 Repository Structure

    LOCAL REPOSITORY                                   REMOTE
    ────────────────────────────────────────────────────────────────────────

    [ Working Directory ]   [ Staging Area (Index) ]   [ Repository (HEAD) ]     [ Repository (HEAD) ]

------------------------------------------------------------------------

## 🔁 Command Flow

### ➕ Adding Changes

    [ Working Directory ]  -- git add -->  [ Staging Area (Index) ]

### 💾 Committing

    [ Staging Area (Index) ]  -- git commit -->  [ Repository (HEAD) ]

### 🚀 Pushing to Remote

    [ Repository (HEAD) ]  -- git push -->  [ Remote Repository (HEAD) ]

------------------------------------------------------------------------

### ⬇ Pulling from Remote

    [ Remote Repository (HEAD) ]  -- git pull -->  [ Repository (HEAD) ]

### ↩ Checking Out Files / Commits

    [ Repository (HEAD) ]  -- git checkout -->  [ Working Directory ]

------------------------------------------------------------------------

## 🧠 Combined Workflow

    LOCAL                                                     REMOTE
    ──────────────────────────────────────────────────────────────────────────

    [ Working Directory ]
            |
            | git add
            v
    [ Staging Area (Index) ]
            |
            | git commit
            v
    [ Repository (HEAD) ]
            |
            | git push
            v
    [ Remote Repository (HEAD) ]


    [ Remote Repository (HEAD) ]
            |
            | git pull
            v
    [ Repository (HEAD) ]
            |
            | git checkout
            v
    [ Working Directory ]

------------------------------------------------------------------------

## ⚡ Quick Summary

    EDIT -> ADD -> COMMIT -> PUSH
    PULL -> CHECKOUT -> EDIT

------------------------------------------------------------------------

## 📌 Key Areas

-   **Working Directory** --- your files on disk
-   **Staging Area (Index)** --- what will go into the next commit
-   **Repository (HEAD)** --- commit history stored locally
-   **Remote Repository** --- server copy (usually `origin`)
