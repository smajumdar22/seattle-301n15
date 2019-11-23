Reference - https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433

Partials come in handy when you want to reuse the same HTML across multiple views. 
Think of partials as functions, they make large websites easier to maintain as you don’t 
have to go and change a piece of text in every page it appears in. Instead, you define that 
reusable bundle of code in a file andinclude it wherever you need it.

Including a partial in EJS is quite straightforward. You use <%- include( PARTIAL_FILE ) %> 
where the partial file is relative to the template you use it in.

Example - 
<!-- views/post.ejs -->
    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8">
        <title>POST_TITLE | Node.js Blog</title>
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">
        <style>
            body {
                padding-top: 20px;
                padding-bottom: 20px;
            }
        </style>
    </head>
    <body>
        <div class="container">
            <%- include('partials/navbar') %>
            <div>
                <h2>POST_TITLE</h2>
                <p>by <a href="#">POST_AUTHOR</a></p>
                <p>POST_CONTENT</p>
                <hr>
            </div>
            <%- include('partials/footer') %>
        </div>
    </body>
    </html>
