### mithril.js
---
https://github.com/MithrilJS/mithril.js

```js
var root = document.body

var root = document.body
m.render(root, "Hello")

m.render(root, "My first app")

m.render(root, m("h1", "My first app"))

m("h1", {class: "title"}, "My first app")

m("main", [
  m("h1", {class: "title"}, "My first app"),
  m("button", "A button")
])

var Hello = {
  view: function(){
    return m("main", [
      m("h1", {class: "title"}, "My first app"),
      m("button", "A button")
    ])
  }
}

m.mount(root, Hello)

var count = 0
var Hello = {
  view: function(){
    return m("main", [
      m("h1", {class: "title"}, "My first app"),
      m("button", {onclick: function() {count++}}, count + " clicks"),
    ])
  }
}
m.mount(root, Hello)

var Splash = {
  view: funciton(){
    return m("a". {href" "#!/hello"}, "Enter!")
  }
}

m.route(root, "/splash", {
  "/splash": Splash,
  "/hello": Hello,
})

var count = 0
var increment = function() {
  m.request({
    method: "PUT",
    url: "//rem-rest-api.herokuapp.com/api/tutorial/1 ",
    data: {count: count + 1},
    withCredentials: true,
  })
  .then(function(data){
    count = parseInt(data.count)
  })
}

var Hello = {
  view: function() {
    return m("main", [
      m("h1", {class: "title"}, "My first app"),
      m("button", {onclick: increment}, count + " clicks")
    ])
  }
}
```

```
```

```
```

