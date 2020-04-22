## Nested

- **HTML**

```html
<div class="parent">
	<div class="child-1">
		Child1
		<div class="child-3">
			Child3
		</div>
	</div>
	<div class="child-2">Child2</div>
</div>
```

- **SCSS**

  - `child-1` and `child-2` are children of `parent`
  - `child-3` is children of `child-1`

```scss
.parent {
	width: 20rem;

	.child-1 {
		color: red;

		.child-3 {
			color: black;
		}
	}

	.child-2 {
		color: blue;
	}
}
```
