# Long Exposure Calculator

A compact, mobile-friendly exposure calculator for pinhole photography and other long-exposure work. Start with a normal meter reading, account for the actual aperture, ISO, filters, and reciprocity failure, and get the final exposure time.

**[Open the calculator](https://wilsmyth-del.github.io/long-exposure-calculator/)**

## Features

- Converts a metered shutter speed and aperture to the camera's actual aperture.
- Accepts a known f-number or calculates it from focal length and pinhole diameter.
- Adjusts for differences between metered ISO and the ISO of the film, paper, X-ray film, or other medium.
- Includes colour-filter and neutral-density filter compensation from 1 to 10 stops.
- Supports reciprocity correction from a known exposure pair or a custom exponent.
- Offers a no-reciprocity mode for digital sensors.
- Shows the calculation step by step.
- Includes a countdown timer for the final exposure.
- Runs entirely in the browser with no installation or server required.

## How to use it

1. Enter the shutter speed, aperture, and ISO from your meter or metering app.
2. Enter the camera's actual f-number, or calculate it from focal length and pinhole diameter.
3. Enter the ISO of the medium you are exposing.
4. Choose a reciprocity method and add any filter compensation.
5. Read the calculated exposure time and use the built-in timer when ready.

The expanded **Working** section shows how each adjustment contributes to the result.

## Reciprocity correction

The calculator can derive a reciprocity exponent from one exposure pair: a metered time and the corrected time recommended for that material. It then applies the relationship:

```text
corrected time = metered time ^ p
```

You can also enter the exponent directly or disable reciprocity correction. Reciprocity behavior varies by material, age, processing, and conditions, so treat manufacturer data and testing as the final authority.

## Run locally

Download or clone the repository, then open `index.html` in a modern browser. The app has no dependencies and does not send data anywhere.

```bash
git clone https://github.com/wilsmyth-del/long-exposure-calculator.git
cd long-exposure-calculator
```

## Project structure

```text
index.html   Complete application: markup, styles, and JavaScript
README.md    Project documentation
```

## Contributing

Bug reports and improvements are welcome. Open an issue or submit a pull request on GitHub.

## License

No license has been specified yet. Unless a license is added, the usual copyright restrictions apply.
