# Useful-Regex
An collection of useful regex

`Guid`:
```
[a-z0-9]{8}[\-][a-z0-9]{4}[\-][a-z0-9]{4}[\-][a-z0-9]{4}[\-][a-z0-9]{12}
```

`Username`:
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
