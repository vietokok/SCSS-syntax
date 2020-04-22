## Parent Selector: &
- `&` đại diện cho phần tử nó nằm trong gần nhất.

- **HTML**

```html
<div class="box">
  <div class="box-text">Demo</div>
</div>
```

- **SCSS**

  - & ở đây đại diện cho phần tử cha gần nhất là `.box`  
  > & bao gồm cả bộ chọn class `.` 
```scss
.box{
  display: inline-block;
  padding: 1rem;
  background-color: #ddd;
  &-text{
    color: red;
  }
  &:hover &-text{
    color: blue;
  }
}
```
