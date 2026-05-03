# my-website-
Upload file-
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mazhar Blog</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f4f4f4;
    }header {
  background: #111;
  color: white;
  padding: 15px;
  text-align: center;
}

nav {
  background: #333;
  padding: 10px;
  text-align: center;
}

nav a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
}

.container {
  padding: 20px;
}

.post {
  background: white;
  padding: 15px;
  margin-bottom: 15px;
  border-radius: 8px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
}

.post h2 {
  margin-top: 0;
}

.add-box {
  background: white;
  padding: 15px;
  border-radius: 8px;
  margin-bottom: 20px;
  box-shadow: 0 0 5px rgba(0,0,0,0.1);
}

input, textarea {
  width: 100%;
  padding: 10px;
  margin-top: 8px;
  margin-bottom: 10px;
}

button {
  padding: 10px 15px;
  background: #111;
  color: white;
  border: none;
  cursor: pointer;
}

footer {
  text-align: center;
  padding: 15px;
  background: #111;
  color: white;
  margin-top: 20px;
}

.whatsapp {
  display: inline-block;
  margin-top: 10px;
  background: green;
  color: white;
  padding: 10px;
  text-decoration: none;
  border-radius: 5px;
}

  </style>
</head>
<body><header>
  <h1>Mazhar Ka Blog</h1>
  <p>Welcome to my personal website</p>
</header><nav>
  <a href="#">Home</a>
  <a href="#posts">Posts</a>
  <a href="#contact">Contact</a>
</nav><div class="container">  <div class="add-box">
    <h2>Add New Post</h2>
    <input type="text" id="title" placeholder="Post Title" />
    <textarea id="content" rows="4" placeholder="Post Content"></textarea>
    <button onclick="addPost()">Publish Post</button>
  </div>  <h2 id="posts">Latest Posts</h2>  <div id="postContainer">
    <div class="post">
      <h2>Mera Pehla Post</h2>
      <p>Yeh mera pehla blog post hai. Main yahan apni updates share karunga.</p>
    </div><div class="post">
  <h2>Website Banane Ka Tareeqa</h2>
  <p>Is post mein main sikha raha hoon ke GitHub Pages se website kaise banate hain.</p>
</div>

  </div><a class="whatsapp" href="https://wa.me/923701037382" target="_blank">Contact on WhatsApp</a>

</div><footer>
  <p>© 2026 Mazhar Blog | All Rights Reserved</p>
</footer><script>
function addPost() {
  let title = document.getElementById('title').value;
  let content = document.getElementById('content').value;

  if(title === '' || content === '') {
    alert('Please fill both fields');
    return;
  }

  let postContainer = document.getElementById('postContainer');

  let newPost = document.createElement('div');
  newPost.classList.add('post');

  newPost.innerHTML = '<h2>' + title + '</h2><p>' + content + '</p>';

  postContainer.prepend(newPost);

  document.getElementById('title').value = '';
  document.getElementById('content').value = '';
}
</script></body>
</html>

