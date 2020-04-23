## @for and @while
  - **@for** 
  
    > to: < end, through: <= length
  
    ```scss
    .demo {
      width: 30rem;
      padding: 1rem;
      background-color: #ddd;
      .content {
        margin: .75rem;
        padding: .75rem;
      }
    }
   
    @for $i from 1 through 4 {
      .content:nth-child(#{$i}) {
        opacity: $i * 0.1;
      }
    }
    ```
    
  - **@while**    
  
    ```scss    
    @while $i < 5 {
      .content:nth-child(#{$i}) {
        opacity: $i * 0.1;
      }
      $i: $i + 1; 
    }
    ```
