# Git Commit

## Guideline
- Write down `Why` &`What` you change your code
- Every commit is related to specific reason
- Don't commit a large changes

## Impacts
- Writ a good commit message is helpful for you or others to maintain the code 

## Example about the convention of a git commit message
- Format of a git commit message
```
<type>:<subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer> 
```

- Allowed `<type>`
    - `Feat`: `Feat`=Feature,  when we add/revise features.
    - `Fix` : when you fix a bug.
    - `Docs`: Add/Revise documentation or append the docstring
    - `Style`: Change some styles like "white space, formatting, missing semi colons, etc"
    - `Refactor`: Not about adding new features and fix the bugs
    - `Perf`: A code change that improves the performance
    - `Test`: When add missing tests
    - `Chore`: maintain, update the requirements about dev/production

- Allowed `subject`
    - don't capitalize first letter

- `<footer>` message
    - About the issue number, like `issue #123` 

## Reference
- [Git Commit Message Conventions](https://docs.google.com/document/d/1QrDFcIiPjSLDn3EL15IJygNPiHORgU1_OOAqWjiDU5Y/edit#heading=h.greljkmo14y0)