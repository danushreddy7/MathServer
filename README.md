# Ex.05 Design a Website for Server Side Processing
## Date:

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
# index.html:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lamp Filament Power Calculator</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Lamp Filament Power Calculator</h1>
        <form id="power-form">
            <div class="input-group">
                <label for="intensity">Intensity (I in Amperes):</label>
                <input type="number" id="intensity" name="intensity" step="0.01" required>
            </div>
            <div class="input-group">
                <label for="resistance">Resistance (R in Ohms):</label>
                <input type="number" id="resistance" name="resistance" step="0.01" required>
            </div>
            <button type="submit">Calculate Power</button>
        </form>
       <div class="result" id="result"></div>
    </div>

   <script>
        document.getElementById('power-form').addEventListener('submit', function(event) {
            event.preventDefault();
            const intensity = parseFloat(document.getElementById('intensity').value);
            const resistance = parseFloat(document.getElementById('resistance').value);
            const power = Math.pow(intensity, 2) * resistance;

            document.getElementById('result').innerText = "Power: " + power.toFixed(2) + " Watts";
        });
    </script>
</body>
</html>

#style.css


## HOMEPAGE:
![image](https://github.com/user-attachments/assets/5f461b00-10df-46b5-b104-c73956897620)




## RESULT:
The program for performing server side processing is completed successfully.
