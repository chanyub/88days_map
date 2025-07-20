# Australia Postcode Map Visualization

An interactive map displaying Australian postcodes with color-coded regions based on different classification tables. Users can search for specific postcodes or localities and explore the geographical distribution of postal areas.

## Features

- **Interactive Map**: Browse Australian postcodes with Leaflet.js
- **Color-coded Regions**: Different tables are represented by distinct colors:
  - Table 1: Red (#ff0000)
  - Table 2: Orange (#ff8c00)
  - Table 3: Yellow (#ffff00)
  - Table 4: Lime Green (#32cd32)
  - Table 5: Blue (#0078ff)
  - Table 6: Purple (#9370db)
- **Search Functionality**: Search by postcode or locality name
- **Click Interaction**: Click on regions to highlight them with darker colors
- **Visitor Statistics**: Track total and daily visitor counts

## Live Demo

[View Live Demo](https://chanyub.github.io/88days_map/)

## Usage

1. Open `index.html` in a web browser
2. Use the search bar at the top to find specific postcodes or localities
3. Click on any region to highlight it
4. Click on empty areas to deselect highlighted regions

## Data Sources

- **Postcode Boundaries**: Australian Bureau of Statistics POA 2021 GeoJSON data
- **Classification Tables**: Six CSV files (table1.csv - table6.csv) containing postcode classifications
- **Locality Names**: Postcode to locality name mappings in JSON format

## File Structure

```
├── index.html              # Main application file
├── poa2021.geojson         # Australian postcode boundary data
├── postcode2name.json      # Postcode to locality name mapping
├── table1.csv             # Classification table 1 (Red)
├── table2.csv             # Classification table 2 (Orange)
├── table3.csv             # Classification table 3 (Yellow)
├── table4.csv             # Classification table 4 (Lime Green)
├── table5.csv             # Classification table 5 (Blue)
└── table6.csv             # Classification table 6 (Purple)
```

## Technologies Used

- **Leaflet.js**: Interactive mapping library
- **OpenStreetMap**: Base map tiles
- **HTML5/CSS3/JavaScript**: Frontend technologies
- **LocalStorage**: Client-side visitor statistics

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/chanyub/88days_map.git
   ```

2. Open `index.html` in a web browser - no server required!

## Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Australian Bureau of Statistics for postcode boundary data
- OpenStreetMap contributors for base map tiles
- Leaflet.js community for the mapping library