<div style:"text-align:center;">
<p>
    <img src="https://badges.frapsoft.com/os/v2/open-source.svg?v=103" alt="NuGet" />
    <a href="#buy-me-a-coffee-" target="_blank"><img src="https://badgen.net/badge/icon/buymeacoffee/green?icon=buymeacoffee&label"/></a>
</p>
</div>

# Useful Regular Expressions

Here I have tried to collect a collection of useful used regexes!

### Username:
```
^(?=.{8,20}$)(?![_.])(?!.*[_.]{2})[a-zA-Z0-9._]+(?<![_.])$

 └─────┬────┘└───┬──┘└─────┬─────┘└─────┬─────┘ └───┬───┘
       │         │         │            │           no _ or . at the end
       │         │         │            │
       │         │         │            allowed characters
       │         │         │
       │         │         no __ or _. or ._ or .. inside
       │         │
       │         no _ or . at the beginning
       │
       username is 8-20 characters long
```

### Guid:
```
[a-z0-9]{8}[\-][a-z0-9]{4}[\-][a-z0-9]{4}[\-][a-z0-9]{4}[\-][a-z0-9]{12}
```

### Email:
```
^[\w-\.]+@([\w-]+\.)+[\w-]{2,4}$
```

## Buy me a coffee :)
