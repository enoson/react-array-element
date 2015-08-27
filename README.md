# react-array-element
JSX:
```js
<div className="comment">
  <h2 className="commentAuthor">
      {this.props.author}
  </h2>
</div>
```
react-array-element:
```js
import $ from 'react-array-element'

$(".comment",
   ["h2.commentAuthor", this.props.author])
```
JSX:

```js
<ComponentA id="email-input"
  style = {style} onClick = {this.onClick} >
  <input
    type="email"
    onKeyUp={ this.onKeyUp } />
</ComponentA>
```
react-array-element:
```js
$("ComponentA#email-input",
  {style, onClick:this.onClick},
  ["input", {
    type:"email",
    onKeyUp: this.onKeyUp }])
```

###No more div,id,className,{},closing tag, just vanilla array.
