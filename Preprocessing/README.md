# Preprocessing hints, scripts etc...

## Javascript "reverse value map"

Simple preprocessor to translate strings to numbers (used with oracle cluster checks):

```
switch(value) {
  case 'ONLINE':
    return 3
    break;
  case 'OFFLINE':
    return 0
    break;
  case 'UNKNOWN':
    return 1
    break;
  case 'INTERMEDIATE':
    return 2
    break;
}
```
