## Mixin & include
- Dùng để tạo một đối tượng và tái sử dụng nó

- **CSS: Các thuộc tính bị lặp lại ở các `class`**  
  
```css
.box1{
  width: 10rem;
  height: 8rem;
  background-color: #ddd;
  border-radius: .5rem;  
}

.box2{
  width: 15rem;
  height: 12rem;
  background-color: #aaa;
  border-radius: .75rem;  
}
```

- **SCSS**

```scss
$bg1: "#ddd";
$bg2: "#aaa";

@mixin box($w, $h, $bc, $br){
  width: $w;
  height: $h;
  background-color: $bc;
  border-radius: $br;  
}

.box1{
  @include box(10rem, 8rem, $bg1, 0.5rem); 
}

.box2{
  @include box(15rem, 12rem, $bg2, 0.75rem);    
}
```
