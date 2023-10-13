---
name: Button click
---

まずは簡単なところからclickで内容が変わるbutton

```html
<button data-hx-get="api/01-button-click.html">
  Let's click
</button>
```

<div style="position:absolute; background:gray; padding:0 0.5rem; border-radius:0.5rem; font-size:0.5rem; color:white">api/01-button-click.html</div>

```html
Clicked
```

<button data-hx-get="api/01-button-click.html">
  Let's click
</button>

<br>
`hx-target`属性で置き換える要素を指定

```html
<button data-hx-get="api/01-button-click.html"
        data-hx-target=".target-01-button-click">
  Let's click
</button>
<span class="target-01-button-click"></span>
```

<button data-hx-get="api/01-button-click.html" data-hx-target=".target-01-button-click">
  Let's click
</button>
<span class="target-01-button-click"></span>

<br>
`hx-trigger`属性で任意のeventと修飾子  
複数指定可能

once修飾子
```html
<button data-hx-get="api/01-button-click.html"
        data-hx-trigger="click once">
  Let's click
</button>
```

<button data-hx-get="api/01-button-click.html" data-hx-trigger="click once">
  Let's click
</button>

delay修飾子
```html
<button data-hx-get="api/01-button-click.html"
        data-hx-trigger="click delay:3s">
  Let's click
</button>
```

<button data-hx-get="api/01-button-click.html" data-hx-trigger="click delay:3s">
  Let's click
</button>

throttle修飾子
```html
<button data-hx-get="api/01-button-click.html"
        data-hx-trigger="click throttle:3s">
  Let's click
</button>
```

<button data-hx-get="api/01-button-click.html" data-hx-trigger="click throttle:3s">
  Let's click
</button>

textareaなどだとdelayとchangedの掛け合わせで[audit](https://rxjs.dev/api/operators/audit)みたいになるっぽい
