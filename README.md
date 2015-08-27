# react-array-element
JSX:
```
<div className="comment">
  <h2 className="commentAuthor">
      {this.props.author}
  </h2>
</div>
```
react-array-element:
```
$(".comment",
   ["h2.commentAuthor", this.props.author])
```
JSX:

```
<ComponentA id="email-input"
  style = {style} onClick = {this.onClick} >
  <input
    type="email"
    onKeyUp={ this.onKeyUp } />
</ComponentA>
```
react-array-element:
```
$("ComponentA#email-input",
  {style, onClick:this.onClick},
  ["input", {
    type:"email",
    onKeyUp: this.onKeyUp }])
```

###No more div,id,className,{},closing tag, just vanilla array.
