# Ex.07 Design of Interactive Image Gallery
# Date:
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
HTML CODE
```
<html>
<head>
    <title>Interactive Image Gallery</title>
    <link rel="stylesheet" href="style.css">

    <script>
        const gallery = [
            { src: "dhoni1 (1).png", caption: "MAHENDRA SINGH DHONI" },
            { src: "virat.png", caption: "VIRAT KOHLI" },
            { src: "rohit.png", caption: "ROHIT SHARMA" },
            { src: "rahul.png", caption: "KL RAHUL" },
            { src: "iyer.png", caption: "SHREYAS IYER" },
        ];

        let index = 0;

        function updateImage()
         {
            document.getElementById("img").src = gallery[index].src;
            document.getElementById("text").innerHTML = gallery[index].caption;
        }

        function next()
         {
            index++;
            if(index >= gallery.length){
               index = 0;
             }
            updateImage();
        }

        function previous()
         {
            index--;
            if(index < 0){
               index = gallery.length - 1;
            }
            updateImage();
        }
    </script>
</head>
<body>
    <div class="title">
        <h1>INTERACTIVE IMAGE GALLERY</h1>
    </div>
    <div class="allign">
        <div class="image">
            <img id="img" src="dhoni (1).png" alt="Gallery Image">
            <h2 id="text">MAHENDRA SINGH DHONI</h2>
            <div class="button1">
                <button onclick="previous()">Previous</button>
                <button onclick="next()">Next</button>
            </div>
        </div>
    </div>
    <footer class="copyrights">
        <h4> &copy; Designed by E HEMACHANDRAN (212224230093)</h4>
    </footer>
</body>
</html>

```
CSS CODE
```
body{
    background-image: url(bg.png);
}

.title {
    height: 60px;
    width: 100%;
    background-color: rgb(146, 115, 176);
    color: black;
    text-align: center;
    line-height: 60px;
    
}

.allign {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 80px;
}

.image {
    width: 320px;
    background-color: lightgray;
    border: 1px solid black;
    border-radius: 12px;
    padding: 20px;
    box-shadow: 0 8px 18px rgba(0, 0, 0, 0.2);

    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 15px;
}

.image img {
    height: 220px;
    width: 200px;
    border-radius: 10px;
    object-fit: cover;
}

.image h2 {
    font-size: 20px;
    margin: 0;
    text-align: center;
}

.button1 {
    display: flex;
    gap: 25px;
}

button {
    background-color: darkgreen;
    color: white;
    padding: 10px 18px;
    font-size: 15px;
    border: none;
    border-radius: 8px;
    cursor: pointer;
}

button:hover {
    background-color: darkgreen;
}

.copyrights {
    background-color: rgb(146, 115, 176);
    color: black;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: 100%;
    font-size: 14px;
    text-align: center;
}

```
# OUTPUT:

<img width="1919" height="1199" alt="Screenshot 2026-05-22 131024" src="https://github.com/user-attachments/assets/73a2bb76-fb53-44e9-9d53-e42a95406d4d" />

<img width="1919" height="1199" alt="Screenshot 2026-05-22 131035" src="https://github.com/user-attachments/assets/e771f5ee-1c75-494a-9adc-4ab947da1488" />

<img width="1913" height="1198" alt="Screenshot 2026-05-22 131046" src="https://github.com/user-attachments/assets/86c221bc-638b-46ff-bad9-198155db5549" />

<img width="1918" height="1199" alt="Screenshot 2026-05-22 131056" src="https://github.com/user-attachments/assets/2c501694-59f3-46b2-8609-363b12fc122c" />

<img width="1919" height="1199" alt="Screenshot 2026-05-22 131016" src="https://github.com/user-attachments/assets/bc3bb37f-c21d-424c-9c57-0f4c959fe32f" />






# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
