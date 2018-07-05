# DOCKER FILES

A collection of any Docker files I'm using on my dev machines / lab / etc.

## RECOMMENDATION

Use aliases to reference containers, so you can use shorthand and just pass in commands. It makes life much easier.

Example (in your .bashrc, .bashprofile, .zshrc, etc)

```
alias frontend-toolkit='docker run -it --rm -p 3000:3000 -v "$PWD":/app -w /app jasonamartin/frontend-toolkit:latest $1'
```

And now in your terminal, you could just run something like this from the directory:

```
frontend-toolkit npm i
```

Another idea is to split up input, so you can pass a working dir and command.

## CONTENTS

/frontend/frontend-toolkit : This is an image spawned from Node with grunt, gulp, webpack, etc built it for fast zero to development setup.
