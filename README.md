# Ex.05 Design a Website for Server Side Processing
# Date:20.04.2025
# AIM:
To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side.

# FORMULA:
P = I2R
P --> Power (in watts)
 I --> Intensity
 R --> Resistance

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Create python programs for views and urls to perform server side processing.

## Step 5:
Create a HTML file to implement form based input and output.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h1 {
            color:rgb(20, 126, 219);
        }
        label {
            color: rgb(8, 6, 3);
            font-size: 150%;
            }
        input {
            font-size: 150%;
        }
        button {
            font-size: 150%;
        }
        p {
            color: rgb(21, 16, 2);
            font-size: 200%;
            }
        body {
            background-color: #cccccc;
        }

        h1{
            border: 2px solid black;
            padding: 20px;
            margin: 10px;
            border-radius: 5px;
            position: fixed;
            top: 200px;
            right: 500px;
            font-size: xx-large;
            font-weight: bolder;
            font-variant: small-caps;
            background: linear-gradient(to bottom,rgb(224, 34, 145),white,rgb(203, 44, 105));
            font-family: Georgia, 'Times New Roman', Times, serif;
            color: grey;
        }
        form{
            border: 2px solid black;
            background-color: rgba(128, 128, 128, 0.064) ;
            padding: 30px;
            margin: 10px;
            border-radius: 10px;
            width: 425px;
            position: fixed;
            top: 300px;
            left: 527px;
        
            background-size: 60%;
            background-repeat: no-repeat;
            background-position: left;
            
        }


    </style>
</head>
<body>
    <h1 align="center">CALCULATION OF POWER</h1>
    <form action="{% url 'power' %}" method="POST">
        {% csrf_token %}
        <label>Intensity: </label>
        <input type="number" name="intensity">
        <br>
        <br>

        <label>Resistance: </label>
        <input type="number" name="resistance">

        <br>
        <br>
        <br>


        <button type="submit">Calculate</button>
        <p align="center">The Power of the lamp is: {{ output }}</p>
    </form>
</body>
</html>
```
# OUTPUT:
![Screenshot 2025-04-22 114506](https://github.com/user-attachments/assets/80a3f757-ac9a-47b6-a500-40bacc0fbc4f)

# RESULT:
The program for performing server side processing is completed successfully.
