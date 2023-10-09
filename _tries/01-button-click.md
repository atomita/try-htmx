---
name: Button click
---

まずは簡単なところからclickで内容が変わるbutton

```html
<button data-hx-get="api/01-button-click.html">
  Let's click
</button>
```

<div class="absolute bg-gray-400 rounded pl-1 pr-1 text-xs">api/01-button-click.html</div>

```html
Clicked
```

<button data-hx-get="api/01-button-click.html" class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-full">
  Let's click
</button>
