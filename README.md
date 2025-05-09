# Ex.08 Design of Interactive Image Gallery
## Date: 09/05/2025
## Name: Saravana Kumar S
## Reg no: 212224220090

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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
    <body>
        <header>
            <h1><font color="black">TOP ANIME</font></h1>
        </header>
        <header>
            <h2><font color="black">2024</font></h2>
        </header>
    </body>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
             background-image: url("anime\ world.webp");
            background-size:cover;
        }

        h1 {
            margin-top: 20px;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 300px;
            height: 200px;
            border: 2px solid #ccc;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery">
        <img src="solo leveling.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="wind breaker.jpg" alt="Image 2" onclick="openModal(this)">
        <img src="kaiju-no-8.jpg" alt="Image 3" onclick="openModal(this)">
        <img src="dan da dan.webp" alt="Image 4" onclick="openModal(this)">
        <img src="ishura.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="one piece.jpg" alt="Image 5" onclick="openModal(this)">
        <img src="blue box.jpg" alt="Image 5" onclick="openModal(this)">
    </div>
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>
    <script>
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>




```

## OUTPUT:

![Screenshot 2025-01-01 111340](https://github.com/user-attachments/assets/d27da855-2a43-4877-aeb5-a3b77ba54663)
![Screenshot 2025-01-01 111430](https://github.com/user-attachments/assets/aa0829a4-208f-4dad-b5b4-2e0a7e65d1b1)
![Screenshot 2025-01-01 111452](https://github.com/user-attachments/assets/cf153fb4-8cbd-4536-ac08-4aa255c4c1cd)
![Screenshot 2025-01-01 111509](https://github.com/user-attachments/assets/d29620ee-a1e7-401b-843d-7502da0262a5)
![Screenshot 2025-01-01 111523](https://github.com/user-attachments/assets/eeea5b0c-39ca-4328-b974-94833775a3c0)
![Screenshot 2025-01-01 111540](https://github.com/user-attachments/assets/d53ae4b9-e192-4ec3-9b68-b4eddd296c56)
![Screenshot 2025-01-01 111601](https://github.com/user-attachments/assets/6ced9b0f-6e06-41b0-9563-4d0bdf05558b)
![Screenshot 2025-01-01 111622](https://github.com/user-attachments/assets/bcde3617-4fed-4096-97e0-c25e82020111)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
