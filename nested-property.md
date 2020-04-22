## Nested Property
- **HTML**

```html
<div class="text">Demo</div>
```

- **SCSS**

  - `font` là từ chung của các thuộc tính
  - `size`, `family`, `weight` là các từ đi kèm
```scss
.text{
  font:{
    size: 2rem;
    family: "Arial";
    weight: bold;
  }
}
```
