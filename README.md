JS Reference Doc
============
## Functions

---

#### `whenPageIsReady`
Executes all the code written inside the function, passed as a parameter, when the page is ready.

```js

function whenPageIsReady(func) {
    // If the page is not loading, it's ready.
    if (document.readyState != 'loading') {
        // Execute the func passed.
        func();
    } else {
        // Wait for the Page to get Loaded and execute the func passed.
        document.addEventListener('DOMContentLoaded', function(){
          console.log("function called");
        });
    }
}

```

#### `click`
Add `addEventListener` to the `element` passed as the parameter.

```js

function click(element, func) {
    if (element) {
        element.addEventListener("click", func(){
            console.log("Listener func called");
        });
    }
}

```

---

#### `onClickMultiple`
Executes the given function if the element has the parameter `className`.

```js

function onClickMultiple(className, func) {
    document.addEventListener('click', function(event) {
        if (event.target.classList.contains(className)) {
            func(event.target);
        }
    });
}

```

---

#### `scrollToBottom`
Scrolls an element to the bottom.

```js

function scrollToBottom(element) {
    element.scrollTop = element.scrollHeight;
}

```

---

#### `redirectTo`
Redirects your browser to the `page` parameter passed.

```js

function redirectTo(page) {
    window.location = page;
}


```

---

#### Get / select an element.
Specify html `id` of the element with a #

```js

var element = getElement('#element');

console.log(element);

```

---

#### Add a class to an element.
Specify html `id` of the element with a #

```js

var element = getElement('#element');

element.classList.add('className');

console.log("Added " + className);

```

---

#### Remove a class from an element.
Specify html `id` of the element with a #

```js

var element = getElement('#element');

element.classList.remove('className');

console.log("Removed " + className);

```

---

#### Set a attribute to an element.
Specify html `id` of the element with a #

```js

var element = getElement('#element');

element.setAttribute('key', value);

console.log("Added attribute" + key + ": " + value);

```

---
