## List and @each
  - **HTML**
  
  ```html
  <div class="nav-20">20%</div>
  <div class="nav-50">50%</div>
  <div class="nav-100">100%</div>
  ```
  
  - **SCSS**
  
  ```scss
  %common {
    height: 1rem;
    text-align: center;
    background-color: #ddd;    
  }
  
  $sizes: 20, 50, 100;
  
  @each $size in $sizes {
    .nav-#{$size} {
      width: $size * 5px;
      @extend %common;
    }
  }
  ```
  
