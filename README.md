# Ex-07-CSS
# AIM
Using CSS media queries, modify the webpage's color scheme with the following requirements:

Default Color Scheme: Background color: Light gray (#f4f4f4) Text color: Dark gray (#333) Link color: Blue (#007bff) Small Screen Adaptation (Max-width: 600px):

Change the background color to dark gray (#333) Change the text color to light gray (#f4f4f4) Change the link color to light green (#28a745)

Dark Mode Preference:

If the user has set their device to dark mode, override the above styles with the following: Background color: Black (#000) Text color: White (#fff) Link color: Cyan (#17a2b8)

# DESIGN STEPS: 7(i)
## Step 1:
Start Define the document type as HTML.

## Step 2:
Open the HTML structure with the necessary head and body sections. In the head section, set the title of the webpage and define the styles for the webpage. The styles include: -->Default color scheme for the webpage. -->Adaptations for small screen sizes. -->Adaptations for users who prefer a dark color scheme.

## Step 3:
In the body section, create a division with the text “Saveetha Engineering College Blocks”. Also in the body section, create a list with links to the computer science and information Technology,Electronics communication and Engineering, and Admin.

## Step 4:
Close the HTML structure.

# CODE:7(i)
```html
<!DOCTYPE html>
<html>
<head>
<style>
    /* Default Color Scheme */
    body {
            background-color: #181157ce;
            color: #333;
        }
        
        a {
            color: #00ff0d;
        }
        
        /* Small Screen Adaptation */
        @media (max-width: 600px) {
            body {
                background-color: #333;
                color: #f4f4f4;
            }
        
            a {
                color: #bac4bc00;
            }
        }
        
        /* Dark Mode Preference */
        @media (prefers-color-scheme: dark) {
            body {
                background-color: #8b962b;
                color: #681414;
            }
        
            a {
                color: #17a2b8;
            }
        }

</style>
</head>
<body>
    <div>
 Saveetha Engineering college blocks
  </div>
    <ul>
        <li><a href="https://colab.research.google.com/">Computer science and Information Technology</a></li>
        <li><a href="https://www.onlinegdb.com/">Electronics communication and Enginnering</a></li>
        <li><a href="https://www.jdoodle.com/online-java-compiler/">Admin</a></li>
  </body>
  </html>
```
OUTPUT:
![Screenshot 2023-12-25 110950](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/558eab66-f2f4-4b2d-9181-bd437b2a867f)

![Screenshot 2023-12-25 173132](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/e058232c-76a4-449f-aeed-4c22f55ecd42)

# Ex-07(ii)-CSS

# AIM
To use a media query in CSS to apply different styles to a webpage for mobile devices (with widths less than 600px) and desktop devices (with widths greater than or equal to 600px) by providing an example CSS snippet to demonstrate your answer.

# DESIGN STEPS:7(ii)
## Step 1:
Start the HTML document and create the root element.

## Step 2:
Inside , create the element and include a < style > element for CSS rules.

## Step 3:
Define CSS rules for desktop devices. Use a media query to define CSS rules for mobile devices.

## Step 4:
Create the element inside , which will contain the webpage content

## Step 5:
Inside , create a

for the heading and an for the list of hyperlinks.

## Step 6:
End the HTML document by closing all open tags.

# CODE: 7(ii)
```html
<!DOCTYPE html>
<html>
<head>
<style>
    /* Default Color Scheme */
    body {
            background-color: #ff0000;
            color: #fa0000;
        }
        
        a {
            color: #a6ad58;
        }
        
        /* Small Screen Adaptation */
        @media (max-width: 660px) {
            body {
                background-color: #ff0000;
                color: #f4f4f4;
            }
        
            a {
                color: #28a745;
            }
        }
        
        /* Dark Mode Preference */
        @media (prefers-color-scheme: dark) {
            body {
                background-color: #52e90dcb;
                color: #5f0000;
            }
        
            a {
                color: #09075a;
            }
        }

</style>
</head>
<body>
     <div>
 Saveetha Engineering College Blocks
  </div>
    <ul>
        <li><a href="https://www.online-python.com/">Computer Science and Information Technology</a></li>
        <li><a href="https://www.programiz.com/">Electronics Communication and engineering</a></li>
        <li><a href="https://www.jdoodle.com/online-java-compiler">Admin</a></li>
  </body>
  </html>
```
OUTPUT:
![Screenshot 2023-12-25 172313](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/e83b8f3e-be85-4ea8-a552-7e36931e53f4)

![Screenshot 2023-12-25 173331](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/5e6e54b4-9892-45ef-a3b4-0883691cf87e)
![Screenshot 2023-12-25 173933](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/28419cd3-0ff7-4888-b3ec-126b1270b6f6)

# Ex-07(iii)-CSS Orientation-based Media Query

# AIM
To explain how you can use CSS media queries to apply different styles based on the orientation (landscape or portrait) of the device. Provide a CSS example where you change the background color of the body based on the orientation.

# DESIGN STEPS:7(iii)
## Step 1:
Identify the section in your HTML file where you want to add the CSS. This is typically within the < style > tags in the section.

## Step 2:
Define a CSS media query for each orientation. The syntax for a media query is @media (orientation: value), where value can be either portrait or landscape.

## Step 3:
Within each media query, specify the CSS rules you want to apply. In this case, you want to change the background color of the body.

## Step 4:
Close the media query with a }.

## Step 5:
Repeat steps 2-4 for the other orientation.

## Step 6:
Save your HTML file.

## Step 7:
Open your HTML file in a web browser and change the orientation of your device to see the different styles applied.

# CODE:7(iii)
```html
!DOCTYPE html>
<html>
<head>
<style type="text/css">
    @media (orientation: portrait) {
        body {
            background-color: rgb(190, 16, 147);
        }
    }

    @media (orientation: landscape) {
        body {
            background-color: rgb(128, 24, 24);
        }
    }
</style>
</head>
<body>
     <div>
   Saveetha Engineering College Blocks
  </div>
    <ul>
        <li><a href="https://www.online-python.com/">Computer Science and Information Technology</a></li>
        <li><a href="https://www.programiz.com/">Electronic Communication and engineering</a></li>
        <li><a href="https://www.jdoodle.com/online-java-compiler">Admin</a></li>
  </body>
  </html>
```
OUTPUT:

![Screenshot 2023-12-25 174657](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/4c964b1e-1f96-473a-9eea-4f766172d6b9)
![Screenshot 2023-12-25 174921](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/03ec71d8-dc31-4149-b430-a420c6b6770b)


# Ex-07(iv)-CSS Responsive Typography
# AIM
To describe how you would use media queries to adjust typography (like font size and line spacing) on a website to improve readability across different device sizes, from mobile phones to large desktop monitors. Include a CSS code snippet in your explanation.

# DESIGN STEPS: 7(iv)
## Step 1:
Identify the HTML elements you want to style. In your case, it’s the div and li elements.

## Step 2:
Identify the HTML elements you want to style. In your case, it’s the div and li elements.

## Step 3:
Use media queries to apply different styles for different device sizes. The @media rule is used in CSS to apply styles for specific media types/devices.

## Step 4:
Inside the media queries, specify the device size for which the styles should apply. You can use min-width and max-width properties to target devices with widths within a certain range.

## Step 5:
Adjust Typography: Inside each media query block, adjust the typography (like font size and line spacing) for the identified elements.

##  Step 6:
Test Your Styles.

## Step 7:
Iterate: Adjust your media queries and styles as needed based on your tests.

# CODE:7(iv)
```html
<<!DOCTYPE html>
<html>
<head>
<style type="text/css">
    div, li {
        font-size: 16px;
        line-height: 1.5;
    }

    @media screen and (min-width: 600px) {
        div, li {
            font-size: 18px;
            line-height: 1.6;
        }
    }

    @media screen and (min-width: 900px) {
        div, li {
            font-size: 20px;
            line-height: 1.7;
        }
    }

    @media screen and (min-width: 1200px) {
        div, li {
            font-size: 22px;
            line-height: 1.8;
        }
    }
</style>
</head>
<body>
     <div>
  Saveetha Engineering College Blocks
  </div>
    <ul>
        <li><a href="https://www.online-python.com/">Computer Science And Information Technology</a></li>
        <li><a href="https://www.programiz.com/">Electronics Communication and Engineering</a></li>
        <li><a href="https://www.jdoodle.com/online-java-compiler">Admin</a></li>
  </body>
  </html>
```
OUTPUT:
![Screenshot 2023-12-25 180037](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/7c1e1a44-c04a-4618-b1be-123dfc7c474f)


![Screenshot 2023-12-25 180119](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/d2f7ffd1-217e-419b-a0b8-d0c4020306ce)

Ex-07(v)-Print-friendly CSS
# AIM
To use a media query to change the styling of a webpage when it is printed, such as changing the background to white and hiding non-essential elements. Provide a CSS example.

# DESIGN STEPS:7(v)
## Step 1:
Identify the HTML elements you want to style. In your case, it’s the div and li elements.

## Step 2:
Define the base styles for these elements. This will be the default styling that applies when no media queries match.

## Step 3:
Use media queries to apply different styles for different media types. The @media rule is used in CSS to apply styles for specific media types/devices.

## Step 4:
Inside the media queries, specify the media type for which the styles should apply. You can use print to target printers.

## Step 5:
Adjust Styles: Inside each media query block, adjust the styles for the identified elements. You can change the background to white and hide non-essential elements.

## Step 6:
Test your styles using the print preview feature in browsers to ensure they work as expected.

## Step 7:
Iterate: Adjust your media queries and styles as needed based on your tests.

# CODE:7(v)
```html
<html>
<head>
<style type="text/css">
    div, li {
        font-size: 16px;
        line-height: 1.5;
    }

    @media print {
        body {
            background-color: white;
        }

        div, li {
            font-size: 12px;
            line-height: 1.4;
        }

        /* Add any non-essential elements you want to hide when printing */
        .non-essential {
            display: none;
        }
    }
</style>
</head>
<body>
     <div>
        saveetha Engineering college Blocks
  </div>
    <ul>
        <li><a href="https://www.online-python.com/">Computer Science And Information Technology</a></li>
        <li><a href="https://www.programiz.com/">Electronics Communication and Engineering</li>
        <li><a href="https://www.jdoodle.com/online-java-compiler">Admin</a></li>
  </body>
  </html>
```
OUTPUT:

![Screenshot 2023-12-25 181341](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/7d23af7d-1911-4069-8519-1bc3b1daae83)

# Ex-07(vi)-Dark Mode Implementation
# AIM
With the increasing popularity of dark mode in user interfaces, explain how you would use a media query to detect if the user has set their system to prefer a dark color scheme. Provide an example of how you would change the background and text colors of a website based on this preference.

# DESIGN STEPS: 7(vi)
## Step 1:
Use the prefers-color-scheme media feature, which is used to detect if the user has requested the system use a light or dark color theme.

## Step 2:
The prefers-color-scheme media feature can have the values light, dark, or no-preference.

## Step 3:
In your CSS, you can use this feature within a @media rule to apply different styles depending on the user’s preference.

## Step 4:
You can set the background color to black and the text color to white when the user prefers a dark color scheme.

## Step 5:
Conversely, you can set the background color to white and the text color to black when the user prefers a light color scheme.

## Step 6:
If the user has no preference, you can choose a default color scheme.

## Step 7:
Remember to test your website in both light and dark modes to ensure the colors work well in both settings.

# CODE: 7(vi)
```html
!DOCTYPE html>
<html>
<head>
<style type="text/css">
    body {
        background-color: white;
        color: black;
    }
    @media (prefers-color-scheme: dark) {
        body {
            background-color: black;
            color: white;
        }
    }
    @media (prefers-color-scheme: light) {
        body {
            background-color: white;
            color: black;
        }
    }
</style>
</head>
<body>
    <div>
   Saveetha engineering College
  </div>
    <ul>
        <li><a href="https://www.online-python.com/">Computer Science and Information Technology</a></li>
        <li><a href="https://www.programiz.com/">Electronics Communication and Engineering</a></li>
        <li><a href="https://www.jdoodle.com/online-java-compiler">Admin</a></li>
  </body>
  </html>
```
OUTPUT:
![Screenshot 2023-12-25 181920](https://github.com/chandru174642/ODD2023-WT-Ex-07-CSS/assets/139841798/0bc0e7fc-84a7-4dd6-b9b5-b817f0867079)

# RESULT:
Therefore the code has been successfully executed.




