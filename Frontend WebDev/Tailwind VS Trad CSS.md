In traditional CSS, we create elements like this:
```html title:Trad.html
<div class="title">
	<h1>Hello World</h1>
</div>
```
and we assign them CSS classes:
```css title:Trad.css
.title{
	font-family: Gotham,
	font-weight: bold
}
```

Here, **title** becomes a custom class pre-defined styles. If we were to rethink this with a utility-first mindset, instead of writing custom class names, we broke styles into small reusable utility classes.

So something like this:
```css title:Tailwind.css
.flex{
	display: flex
}

.items-center{
	align-items: center
}

.text-blue{
	color: blue
}

.text-sm{
	font-size: 12px
}
```

So now our code will look like this:
```html title:Tailwind.html
<div class="flex items-center">
	<h1 class="text-blue">Hello World</h1>
</div>
```

Instead of building pre-defined styles for classes, we translate styles directly to classes. This will save you lots of time as you won't have to worry about naming classes, or structuring styles. While arguably, inline CSS does the same, it doesn't let you code media queries, and advanced properties like pseudo classes.