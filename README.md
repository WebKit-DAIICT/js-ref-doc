JS Reference Doc
============
## Functions

---

#### `whenPageIsReady`
Executes all the code written inside the function, passed as a parameter, when the page is ready.

---

#### `getElement`
Get element based on the parameter `selector`.

---

#### `click`
Add `addEventListener` to the `element` passed as the parameter.

---

#### `onClickMultiple`
Executes the given function if the element has the parameter `className`.

---

#### `scrollToBottom`
Scrolls to the bottom of the given element.

---

#### `redirectTo`
Redirects your browser to the `page` parameter passed.

---

#### `scrollToLatestMessage`
Scroll to the Latest Message

---

#### `ifUserIsLoggedIn`
If User is logged in, executes the function callback given as a parameter.
Else call `redirectTo` with `index.html` as parameter.

---

#### `renderChatPage`
Render the chat page
  - Hide Page loader
  - Display Chat Area
  - Update page with user data

---

#### `updatePageWithUserData`
Update page with logged in user data based on `user` object passed as parameter.

---

#### `logoutUser`
Logout the current user.

---

#### `createUser`
Create new user in the firebase based on `user` object passed as parameter.

---

#### `loadMembers`
Fetch users list from firebase and executes the function callback passed as parameter.

---

#### `makeMemberItem`
Create member html element to be attached in the members area.
Element is created based on the `member` object passed as parameter.

---

#### `getUser`
Get user data based on his `uid` passed as parameter.

---
