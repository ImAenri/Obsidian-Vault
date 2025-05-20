Tailwind uses JIT or Just-In-Time compiler to modify custom attributes of classes in real time.

Say you want to set a text's size to 13px, Tailwind doesn't have a utility class for that, but you can do so by enclosing the attribute in square brackets

```html title:JIT.jsx
<p class="text-[13px]"> Hello World! </p>
```

And that will display the assigned attribute correctly. It's not only limited to just text sizes though, you can customize just about anything should you wish to do so.

```html title:JIT.jsx
<h1 class="text-[#FFEF89]"> Change Text Color </h1>
<h1 class="bg-[#122831]"> Change Background Color </h1>
<h1 class="h-[1080px]"> Change Height </h1>
<h1 class="before:content-['jsm']"> Change Content </h1>
```

