## Extend
  - Sử dụng `@extend` để kế thừa thuộc tính của một `placeholder`, `class` hoặc `id`.
  
  - Cách tạo một `placeholder`:
  ```scss
  %box {
    width: 10rem;
    height: 5rem;
    line-height: 5rem;
    border-radius: .5rem;
  }
  ```
  
  - Example 
  ```scss
  .box1 {
    width: 10rem;
    height: 5rem;
    line-height: 5rem;
    border-radius: .5rem;
    &-text{
      font-size: 2rem;
      color: deeppink;
    }
  }
  
  .box2{
    @extend .box1;
    &-text{
      @extend .box1-text;
    }
  }
  
  ```

