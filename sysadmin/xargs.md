# xargs

### Usage
```
echo "foo" | xargs -i echo {} "bar"
```
Prints `foo bar`

### Find files and untar them

```
find . -name "*.tar.gz" | xargs -I {} tar xvf {}
```
