## If Else

```scss
@mixin box($w, $h, $bc, $br, $br: false){
  width: $w;
  height: $h;
  background-color: $bc;
  @if $br == true {
     border-radius: 50%;  
  }
  @else {
    border-radius: $h / 10;  
  } 
}
```
