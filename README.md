# Ex.08 Design of Interactive Image Gallery
## Date:12-05-25

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<html>
<head>
    <title>Hari Nivedhan P</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #6c92fb;
            margin: 0;
            padding: 0;

        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            padding: 20px;
            justify-content: center;
        }

        .gallery-item {
            margin: 20px;
            width: 300px;
            height: auto;
            cursor: pointer;
            border-radius: 15px;
            border: 2px solid #e9e9e9;
            transition: transform 0.01s;
        }

        .gallery-item:hover {
            transform: scale(1.2);
        }

        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            max-width: 80%;
            max-height: 80%;
        }

        .close {
            position: absolute;
            top: 20px;
            right: 30px;
            font-size: 30px;
            color: rgb(167, 61, 61);
            cursor: pointer;
        }

        .back {
            background-color: rgb(255, 237, 137);
        }
    </style>
    <script>
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = "flex";
            modalImg.src = image.src;
        }
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = "none";
        }
    </script>
</head>

<body class="back">

    <h1 align="center" style="font-family: Georgia, 'Times New Roman', Times, serif;color: rgb(0, 0, 0);">
        Hari Nivedhan P
        (24013287)</h1>
    <div class="gallery">
        <br><br><br>
        <img src="1.webp" alt="Image 1" class="gallery-item" onclick="openModal(this)" style="position: absolute; top: 100; right: 200;">
        <img src="2.webp" alt="Image 2" class="gallery-item" onclick="openModal(this)" style="position: absolute; bottom: 100; right: 200;">
        <img src="3.webp" alt="Image 3" class="gallery-item" onclick="openModal(this)" style="position: absolute; top: 100; left: 200;">
        <img src="4.webp" alt="Image 4" class="gallery-item" onclick="openModal(this)" style="position: absolute; bottom: 100; left: 200;">
        <img src="5.webp" alt="Image 5" class="gallery-item" onclick="openModal(this)" style="position: absolute; top: 200; right: 550;">
        
    </div>
    <div id="imageModal" class="modal" onclick="closeModal()">
        <span class="close">&times;</span>
        <img class="modal-content" id="modalImage">
    </div>

</body>
```
## OUTPUT:
![alt text](<Screenshot 2025-05-12 105020.png>)

![alt text](<Screenshot 2025-05-12 105036.png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
