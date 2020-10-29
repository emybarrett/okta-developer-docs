The following code is included in the Glitch project templates and includes basic npm packages to define routine tasks for a Node.js application, including listening for requests:

 * Default Code

```javascript
const express = require('express');
const bodyParser = require('body-parser');
```

The following code listens for HTTPS requests:

```javascript
const listener = app.listen(process.env.PORT, () => {
  console.log("Your app is listening on port " + listener.address().port);
});
```