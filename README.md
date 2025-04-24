# Icecast Stream Bandwidth Calculator

A simple, user-friendly web tool to calculate listener capacity for Icecast audio streams based on bitrate and available bandwidth.
https://mbuholzer.github.io/streamcalculator/

## Description

This calculator helps internet radio station operators and audio streamers determine how many concurrent listeners their server can support based on their monthly bandwidth limits and audio bitrate settings.

The tool provides instantaneous results for various listening patterns, helping you make informed decisions about your streaming infrastructure and bandwidth requirements.

## Features

- Calculate listener capacity based on bitrate and monthly bandwidth limit
- Support for common bitrate presets (96, 128, 192, 256 kbit/s)
- Custom bitrate option for specific requirements
- Results for multiple listening patterns (1, 3, 6, 12, and 24 hours per day)
- Custom listener calculator for specific listening hour scenarios
- Responsive design that works on desktop and mobile devices
- Clean, intuitive interface with visual styling

## How It Works

The calculator uses the following formula to determine listener capacity:

1. Calculate data usage per hour: `(bitrate * 60 * 60) / (8 * 1024)` MB
2. Calculate monthly data usage per listener: `(dataPerHour * hoursPerDay * 30) / 1024` GB
3. Calculate maximum listeners: `bandwidthInGB / dataPerMonthPerListener`

## Usage

1. Select your audio stream's bitrate (or input a custom value)
2. Enter your monthly bandwidth limit in TB
3. Click "Calculate Listener Capacity"
4. View the results table showing listener capacity for different listening patterns
5. Use the custom calculator section to test specific listening hour scenarios

## Installation

No installation required! This is a standalone HTML file that works in any modern web browser.

### To run locally:

1. Clone this repository:
`git clone https://github.com/mbuholzer/streamcalculator.git`
2. Open `index.html` in your web browser

### To deploy to your website:

Simply upload the `index.html` file to your web server.

## Technical Details

- Pure HTML, CSS, and JavaScript with no external dependencies
- Lightweight (<50KB total)
- Works offline once loaded
- Compatible with all modern browsers

## Why This Tool?

When planning an internet radio station or any audio streaming service, understanding bandwidth requirements is crucial. Bandwidth costs can be substantial, and this calculator helps you:

- Plan your server infrastructure
- Determine appropriate hosting packages
- Make informed decisions about audio quality vs. listener capacity
- Budget accurately for bandwidth expenses

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Contact

Michael Buholzer
Project Link: https://github.com/mbuholzer/streamcalculator
