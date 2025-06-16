## Inline [[HTML]] Handlers:
```html 
<button onclick = "alert('button clicked!')">Click Me</button>
```

## DOM Property Handlers:
``` js
let btn = document.getElementByID("myButton");
btn.onclick = () => {
	alert("Button Clicked");
}
```

## addEventListner() (Preferred)
``` js
btn.addEventListner("click", () => {
	alert("Button Clicked!");
})
```
addEventListner() is the most versatile as it supports multiple event listners.

## Applications:
1. [[Form Validation]]
2. Dynamic content
3. Interactive lists