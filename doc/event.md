### Events
Event listeners can be registered and unregistered to nodes, listeners are called when an event is published to a node. Some events are published to multiple nodes, but they are not automatically published to parent or children nodes.

```javascript
// Register a listener to node
// Event `name` can be one or an array of strings or spaced separated strings
node.on(name, listener);

// Unregister a listener from node.
node.off(name, listener);

// Get listeners registered to node
// Returns an array or undefined
node.listeners(name);

// Call listeners with args
// Returns number of listeners called
node.publish(name, args);
```
