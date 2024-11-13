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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1 align="center">Calculating Power of a Lamp</h1>
    <form action="{% url 'Result' %}" method="post">
        {% csrf_token %}
       
   <label for="">Intensity : </label>
        <input type="text" name="intensity-input">

   <br>

   <label for="">Resistance : </label>
        <input type="text" name="resistance-input">

   <br>

   <button type="submit">Calculate</button>

   </form>  
</body>
</html>

## HOMEPAGE:
![image](https://github.com/user-attachments/assets/5f461b00-10df-46b5-b104-c73956897620)




## RESULT:
The program for performing server side processing is completed successfully.
