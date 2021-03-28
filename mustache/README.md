## Mustache 复刻

### 如何创建 DOM

原生 API 创建 DOM：

```js
const $nav = document.createElement('div')
const $item = document.createElement('a')
$item.href = 'https://octopandas.github.io'
$item.textContent = 'My Profile'
$nav.appendChild($item)
```

刀耕火种的字符串拼接：

```js
var link = 'https://octopandas.github.io'
var element = [
  '<div>',
  '  <a href="' + link + '">My Profile</a>',
  '</div>'
].join('')
document.getElementById('target').innerHTML += element
```

ES2015 模板字符串：

```js
const element = `
  <div>
    <a href="${link}">My Profile</a>
  </div>
`
```
