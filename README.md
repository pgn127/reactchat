
## Part 2: Multi-room chat - `client/index.js`

Next, we'll implement multiple rooms with a separate component (on the same level as `<ChatRoom />`) called `<ChatRoomSelector />` that will allow us to change which room we are currently chatting with. Note that you will be hard-coding values for room names. The end result will look like the following:

<img src="img/chat2.png" width="600">


## Challenge: "User is typing" 🏆

Create new events in `server.js` called `typing` and `stop typing` that handles received `typing` and `stop typing` events and emits the same events to the rest of the room.

You will also need to change your `client/index.js` to emit a `typing` event when the user is typing (or when `this.state.message` is not empty!) and a `stop typing` event when they are not! Handle the display logic accordingly by updating the `state` of your `<ChatRoom />` to include an array of typing users and rendering with `<span>` items of each typing user with "_username_ is typing..."

The end result will look like the following:

<img src="img/chat3.png" width="600">

Good luck!

## Final Product

Here's a sample of the final product. Feel free to design the entire layout on your own.

![img/User1.png](img/User1.png)
