# Ex.08 Design of Interactive Image Gallery
# Date:09-05-2025
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000000;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            padding: 20px;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 10px;
            cursor: pointer;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.5);
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
    <br>
    <br>
    <br>

    <h1 style="text-align: center; margin-top: 20px; color: #fff;">Interactive Photo Gallery</h1>
    <h3 style="text-align: center; margin-top: 20px; color: #fff;">YUVAN SHANKAR M (24900656)</h3>
     <br>
     <br>
     <br>
     <br>
     <br>

    <div class="gallery">
        <div class="gallery-item" data-image="image1.jpg">
            <img src="Hardik pandya.webp" alt="Photo 1" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image2.jpg">
            <img src="Jaddu.jpg" alt="Photo 2" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image3.jpg">
            <img src="MSD.jpg" alt="Photo 3" onclick="openModal(this)">
        </div>
        <div class="gallery-item" data-image="image3.jpg">
          <img src="rohit sharma.jpg" alt="Photo 3" onclick="openModal(this)">
      </div>
      <div class="gallery-item" data-image="image3.jpg">
        <img src="Suresh Raina.jpg" alt="Photo 3" onclick="openModal(this)">
    </div>
    <div class="gallery-item" data-image="image3.jpg">
      <img src="Virat-Kohli.jpeg" alt="Photo 3" onclick="openModal(this)">
  </div>
        
    </div>

    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        function openModal(image) 
        {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }
        function closeModal() 
        {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>

</body>
</html>

```
# OUTPUT:

![Screenshot (6)](https://github.com/user-attachments/assets/9c911a0c-dfba-4fad-9dfa-51781cdeaf90)
![Screenshot (7)](https://github.com/user-attachments/assets/30e2c3ac-0261-4e76-a8ae-3d4f916b006f)
![Screenshot (8)](https://github.com/user-attachments/assets/56620456-f2d9-4b76-80c4-a8b18f8e3aab)
![Screenshot (9)](https://github.com/user-attachments/assets/95dbb975-6daf-49ff-a599-ad323481aa11)
![Screenshot (10)](https://github.com/user-attachments/assets/bc208ef3-4249-42f7-97cb-1e5c5fd63ec8)
![Screenshot (11)](https://github.com/user-attachments/assets/8b661d34-ee30-419f-bf58-d68a25432251)
![Screenshot (12)](https://github.com/user-attachments/assets/14e327b0-3003-4652-9b89-fb79b89c203c)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
