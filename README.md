# iModal
i-Ready modal framework

# Usage :
## basic modal
```js
iModal.showModal({
    "useInnerHTML": false,
    "title" : "Welcome!",
    "description" : "This is a demo of iModal.",
    "callback" : iModal.closeModal,
});
```

## basic multi-page modal
```js
iModal.showModal({
    "useInnerHTML": false,
    "title" : "page 1",
    "description" : "this is page 1.",
    "callback" : function () {
        iModal.closeModal()
        iModal.showModal({
            "useInnerHTML": false,
            "title" : "page 2",
            "description" : "this is page 2.",
            "callback" : iModal.closeModal,
        })
    },
});
```
