# Ex.08 Design of Interactive Image Gallery
## Date:16.10.2025

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
    <title>Naruto</title>
</head>
<body style="margin:0; font-family: Arial, sans-serif; background-color:#eaf6ff;">
    <header style="text-align: center; background-color: #5ab996; color: white; padding: 1rem 0;">
        <h1>Naruto and friends</h1>
    </header>

    <div style="white-space: nowrap; overflow-x: auto; padding: 1rem; text-align:center;">
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="naruto1.jpg" alt="naruto Group 1" style="height: 200px; border-radius: 10px;">
        </div>
        <div style="display: inline-block; margin-right: 10px;" onclick="openModal(this)">
            <img src="naruto2.jpg" alt="naruto Group 2" style="height: 200px; border-radius: 10px;">
        </div>
        <div style="display: inline-block;" onclick="openModal(this)">
            <img src="naruto3.jpg" alt="narutoGroup 3" style="height: 200px; border-radius: 10px;">
        </div>
    </div>

    <!-- Image Modal -->
    <div id="modal" style="display: none; position: fixed; z-index: 1; left: 0; top: 0; width: 100%; height: 100%; background-color: rgba(0,0,0,0.9);">
        <span style="position: absolute; top: 15px; right: 35px; color: white; font-size: 40px; font-weight: bold; cursor: pointer;" onclick="closeModal()">&times;</span>
        <img id="modalImage" style="display: block; margin: 5% auto; max-width: 80%; border-radius: 15px;">
    </div>

    <script>
        function openModal(element) {
            var modal = document.getElementById("modal");
            var modalImg = document.getElementById("modalImage");
            modal.style.display = "block";
            modalImg.src = element.querySelector("img").src;
        }

        function closeModal() {
            document.getElementById("modal").style.display = "none";
        }
    </script>
</body>
</html>
```

## OUTPUT:
<img width="1919" height="431" alt="Screenshot 2025-10-12 155442" src="https://github.com/user-attachments/assets/3790a7bb-ee61-4ff4-ba40-7896c86a705e" />


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
