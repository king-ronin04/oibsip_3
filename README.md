# oibsip_3 
# Temperature Converter

This is a simple temperature converter that allows the user to convert between Celsius, Fahrenheit and Kelvin temperature units.

## Usage

The user can enter a temperature value in any of the three inputs - Celsius, Fahrenheit or Kelvin. As soon as a value is entered or changed, the values for the other two units will be calculated and updated automatically using the conversion formulas.

For example, entering 100 in the Fahrenheit input will automatically update the Celsius input to 37.78 and the Kelvin input to 310.93.

The allowed range is from -459.67 Fahrenheit (-273.15 Celsius, 0 Kelvin) up to any positive value.

## Working

- index.html - Contains the HTML markup for the inputs and page structure

- style.css - Styles the page elements including fonts, colors, layout etc.

- script.js - Contains the main logic:

  - Get references to the input elements

  - Loop through each input and attach input event listener

  - When an input changes, get the value, determine which input changed 
    using event.target.name

  - Based on input, calculate and update the other temperature values using the
    appropriate conversion formula

  - Conversion formulas used:

    - Celcius to Fahrenheit: F = C * 1.8 + 32
    - Fahrenheit to Celcius: C = (F - 32) / 1.8 
    - Celcius to Kelvin: K = C + 273.15
    - Kelvin to Celcius: C = K - 273.15
    - Fahrenheit to Kelvin: K = (F - 32)/1.8 + 273.15
    - Kelvin to Fahrenheit: F = (K - 273.15) * 1.8 + 32

## Features

- Automatically converts between temperature scales on input
- Responsive design works on all device sizes
- Allows range from absolute zero to any positive value
- Input fields dynamically update with converted values
- Minimal and user-friendly interface

## Potential Improvements

- Add input validation/error handling
- Improve accessibility 
- Support locale formatting of numbers
- Add toggle between Celsius and Fahrenheit as primary units
