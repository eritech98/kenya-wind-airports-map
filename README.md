
# Kenya Wind & Airport Visualization

An interactive **MapTiler-based** web map focused on **visualizing wind patterns** and **airport locations across Kenya**, with **satellite imagery**, **responsive design**, and **tooltip popups** for quick insights. Built for developers, meteorologists, and aviation analysts to explore wind patterns and key airports in Kenya.

## Table of Contents

1. [Features](#features)
2. [Demo Preview](#demo-preview)
3. [Built With](#built-with)
4. [Key Files & Structure](#key-files--structure)
5. [Folder Structure](#folder-structure)
6. [Setup Instructions](#setup-instructions)
7. [License](#license)
8. [Author](#author)

## Features

- Real-time or simulated **wind visualization**
- **Kenyan airports** clearly marked with tooltips for details
- **Satellite imagery** integration
- **Interactive tooltips** displaying airport details on hover
- Fully **responsive design** for both mobile and desktop users
- Focused entirely on **Kenya's geography** and airspace

## Demo Preview

### Interactive Map Interface
![Map Interface](/assets/demo/map1.PNG)

### Wind Visualization Layer
![Wind Layer](/assets/demo/map3.PNG)

### Airport Tooltips in Action and satellie imagery
![Airport Tooltips](/assets/demo/map2.PNG)

## Built With

- **MapTiler** – for high-quality map rendering and satellite layers
- **Leaflet.js** – for interactive mapping and marker management
- **Node.js** – for backend server handling and API integration
- **Express.js** – for routing and serving the app
- **EJS** – for rendering dynamic content in the frontend
- **CSS/Bootstrap** – for responsive styling and UI components

## Key Files & Structure

- `app.js`: The main server file, setting up the Express server and handling API routes.
- `index.ejs`: Frontend view that integrates MapTiler and wind visualization features.
- `.env`: Stores sensitive configuration like the **MapTiler API key** and server port settings.
- `index.js` (in the JS folder): Manages map rendering logic, wind data fetching, and interactive tooltips.
- `styles.css`: Custom styling to ensure responsive and modern design.
- `partials/header.ejs`: Contains the header for the layout, included in the main view.
- `partials/footer.ejs`: Contains the footer for the layout, included in the main view.

## Folder Structure

```bash
├── app.js                # Express server and routes
├── views/                # Contains EJS view files
│   ├── index.ejs         # Main HTML view with MapTiler integration
│   ├── partials/         # EJS partials for reusable components
│   │   ├── header.ejs    # Header partial for the app
│   │   └── footer.ejs    # Footer partial for the app
├── .env                  # Configuration file for environment variables (API keys, port)
├── public/               
│  
│   ├── css/              
│   │   └── styles.css    # Custom styles
│   └── js/               
│       └── index.js      # JavaScript for map rendering and interactivity
├── assets/           
│   └── demo/        
│       ├── map1.png   # Preview of the map interface
│       ├── map2.png    # Preview of wind layer
│       └── map3.png    # Example of airport tooltips
└── package.json                # Project dependencies and scripts

          # Project dependencies and scripts
```

## Setup Instructions

To run this project locally, follow these steps:

### 1. Clone the repository

```bash
git clone https://github.com/eritech98/kenya-wind-airports-maps.git
cd kenya-windmap-airports-maps
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the root directory and add the following:
N/B:Please note in the index.js code, you will be required to put your apiKey
```ini
YOUR_MAPTILER_API=your_maptiler_api_key
PORT=3000
```

### 4. Run the app

```bash
nodemon app.js
```

Then open [http://localhost:3000](http://localhost:3000) in your browser to view the app in action.

## License

This project is licensed under the **MIT License**. Feel free to fork and contribute, but please credit the original author for use in any derivative works.

## Author

**Erick Olando**  
[LinkedIn](https://www.linkedin.com/in/erick-olando-9a9148220) • [Portfolio](https://erick.up.railway.app/) • [Email](mailto:olandoerick98@gmail.com)
