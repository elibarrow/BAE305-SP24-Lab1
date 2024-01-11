# Lab Report 1: Knowing Your Instruments 
Eli Barrow & Issac Stevens      
Jan. 10, 2024


## Summary of Lab
The project goal of this lab was to become comfortable with the lab equipment that we will be using all semester, we experiemented with a power supply, oscilliscope, a function generator, and a Fluke DMM. We began the lab by determining the expected, maximum, and minimum values of resistors using the Fluke DMM. We then did the same type of experimenting with Capacitors to find the expected, maximum, and minimum capacitance of each capacitor we were given. Next we began to work with the o-scope, function generator and power supply to run various different tests. By the end of the lab I am certain that Issac and I are definetley more comfortable using the lab equipment now than before beginning the lab.


## Lab Assignment Specific Items
*Question 1:*    

****Resistor Measurements****
| Color Code | Expected Resistnace k&Omega; | MAX | MIN | Measured | Range |
|:---|:---:|:---:|:---:|:---:|---:|
|   Red-Black-Red-Gold     | 2   |2.1 | 1.9 | 1.966 | In Range |
| Brown-Red-Yellow-Gold    | 120 |126 | 114 | 120.20| In Range |
| Brown-Black-Ornage-Gold  | 10  |10.5| 9.5 | 9.9   | In Range |
| Orange-Orange-Green-Gold |3300 |3465 |3135 | 3500 | Out of Range |



This report includes text and also figures that I linked from my repository.
Like this:
![A test image](https://github.com/cjarro-uky/BAE305-SP24-Lab1/blob/main/20240110_100436.jpg)

Or perhaps a nicer smaller, centered image like this (using html):

<p align="center">
  <img src=https://github.com/cjarro-uky/BAE305-SP24-Lab1/blob/main/20240110_100436.jpg width=50%>
</p>

Also I can include math functions like this:

$$V(V) = I(A)*R(&Omega;)$$

$$P = I^2*R$$

Also I have to include code like this:

```c++
void recvWithEndMarker() {
    static byte ndx = 0;
    char endMarker = '\n';
    char rc;
    
    while (mySerial.available() > 0 && newData == false) {
        rc = mySerial.read();

        if (rc != endMarker) {
            receivedChars[ndx] = rc;
            ndx++;
            if (ndx >= numChars) {
                ndx = numChars - 1;
            }
        }
        else {
            receivedChars[ndx] = '\0'; // terminate the string
            ndx = 0;
            newData = true;
        }
    }
}
```
Also I can make **bold** and *emphatic* statements and add tables like this:

| Variable | Value |
|:---:|---|
|   V      | 5 V   |
| R        | 1 k&Omega; |
| I        | 5 mA  |

Check out these links:

[Link for images](https://docs.github.com/en/communities/documenting-your-project-with-wikis/editing-wiki-content)

[Link for code](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-and-highlighting-code-blocks)

[Link for tables](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables)
