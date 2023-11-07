---
external: false
draft: true
title: Starship
description: Configuring Starship prompt.
date: 2023-11-13
---

## Command Prompt
One of the first things I suggest people do when they start with a terminal 
emulator is to customize the command prompt.  I think it is essential, 
especially for those who are not super comfortable with the terminal, to 
give some more information.  The aesthetics can also be improved dramatically.

[Starship](https://starship.rs/) is my favorite command prompt, it's super 
simple and very aesthetically pleasing.  It is very minimalist with only the
necessary information.  

### Starship config
```toml
# Get editor completions based on the config schema
"$schema" = 'https://starship.rs/config-schema.json'

# Inserts a blank line between shell prompts
add_newline = false

[directory]
style = "blue bold"

# Disable the package module, hiding it from the prompt completely
[package]
disabled = true
[username]
disabled = true
[hostname]
disabled = true
[aws]
disabled = true
[docker_context]
disabled = true
[git_branch]
disabled = false
[git_commit]
disabled = true
[git_state]
disabled = true
[git_metrics]
disabled = true
[git_status]
disabled = true
```

