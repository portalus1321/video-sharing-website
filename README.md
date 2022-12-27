<!DOCTYPE html>
<html>
<head>
  <title>My Video Sharing Website</title>
  <style>
    /* Add some basic styling for the website */
    body {
      font-family: sans-serif;
    }
    h1 {
      text-align: center;
    }
    table {
      border-collapse: collapse;
      width: 80%;
      margin: 0 auto;
    }
    th, td {
      border: 1px solid #dddddd;
      text-align: left;
      padding: 8px;
    }
    tr:nth-child(even) {
      background-color: #dddddd;
    }
    .upload-form {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 20px;
    }
    .upload-form label {
      margin-bottom: 10px;
    }
    .upload-form input[type="submit"] {
      margin-top: 10px;
      padding: 10px 20px;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    .upload-form input[type="submit"]:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <h1>My Video Sharing Website</h1>

  <!-- Add a form for uploading videos -->
  <div class="upload-form">
    <form action="/upload" method="post" enctype="multipart/form-data">
      <label for="videoFile">Select a video to upload:</label><br>
      <input type="file" name="videoFile" id="videoFile"><br>
      <input type="submit" value="Upload">
    </form>
  </div>

  <!-- Add a table for displaying a list of uploaded videos -->
  Copy code
<table>
  <tr>
    <th>Video thumbnail</th>
    <th>Video title</th>
  </tr>
  <tr>
    <td><img src="/videos/thumbnail1.jpg" alt="Video thumbnail"></td>
    <td><a href="/videos/video1.mp4">Video 1</a></td>
  </tr>
  <tr>
    <td><img src="/videos/thumbnail2.jpg" alt="Video thumbnail"></td>
    <td><a href="/videos/video2.mp4">Video 2</a></td>
  </tr>
  <!-- Add more rows for additional videos -->
</table>
