[TOC](Readme.md) [Prev](stringlit.md) [Next](scopes.md)

# Bytes

CUE distinguishes between a `string` and a `bytes` type.
Bytes are converted to base64 when emitting JSON.
Byte literals are defined with single quotes.
The following additional escape sequences are allowed in byte literals:

    \xnn    // arbitrary byte value defined as a 2-digit hexadecimal number
    \0nnn   // arbitrary byte value defined as a 3-digit octal number


<!-- CUE editor -->
```
a: '\x03abc'
```

<!-- JSON result -->
```json
{
    a: "A2FiYw=="
}
```