## The way to format the string

way#1
``` python
"....{}...".format(<variable>)
```
way#2 (3.6+)
``` python
"f...{<variable>}..."
```

## format mini language
inside the {}, we can specify some format rules. please checkout: https://docs.python.org/3.6/library/string.html#format-string-syntax

It is {[field_name] ["!" conversion] [":" format_spec]} in short.

"field name" is the variable name and format spec please checkout:https://docs.python.org/3.6/library/string.html#format-specification-mini-language
