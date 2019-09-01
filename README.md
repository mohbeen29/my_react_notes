# My React Common Errors and Notes


## Common Errors 

### ERROR: Adjacent JSX elements must be wrapped in an enclosing tag. Did you want a JSX fragment <>...</>? (8:6)

Meaning:
Example of issue:

```
function titles(props){
    return (
        <p>One</p>
        <p>Two</p>
    )
}
```

General way to fix it:

Fixed example:

```
function titles(props){
    return (
        <div>
            <p>One</p>
            <p>Two</p>
        </div>
    )
}
```
