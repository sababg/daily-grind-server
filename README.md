# Build a Basic Express.js Server

## Reflections

1: res.send: Sends a response body of any type (string, JSON, HTML) to the client while res.sendFile sends a file to the client. You must provide the absolute path.

2: It makes our file paths absolute because it is possible the relative file pass won't work when we are starting the project.

3: We just follow the same pattern as the dashboard and contact page. Inside the public folder we need to create a Html file and in the server.js we need to create a route for it like contact

```js
app.get("/contact", (req, res) => {
  res.sendFile(path.join(__dirname, "public/contact.html"));
});
```

for easier access for user we need to add a link to other html file, which user click on it to show her the correct route for it.

##

👤 Author
Saba Beigi
🌎 Charlotte, NC
💼 GitHub @sababg
📧 beigisaba@gmail.com

Feel free to reach out with questions, feedback, or ideas!
