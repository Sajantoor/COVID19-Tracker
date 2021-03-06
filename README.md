# Coronavirus Tracker
![COVID-19 Tracker Screenshot](../readme-assets/pictures/Logo.png)

#### Table of Contents
 * [About](#About)
 * [Motivation](#Motivation)
 * [Technologies](#Technologies)
 * [Future Features](#Future-Features)
 * [Getting Started](#Getting-Started)
 * [Contributions](#Contributions)

## About
> The Coronavirus Tracker project is used to visualize and track the COVID-19 (Coronavirus) pandemic. The goal of the project is making information about COVID-19 easily accessible and easy to understand for the public using data visualization. In its current state, the project features a scatterplot layer which changes colors based of the data point and a heat map layer which is weighted based of the value of the data point. It also features the ability to turn these layers on and off, switch between different data parameters such as confirmed cases or deaths and features a tooltip UI component which appears when the user hovers over an element.

#### Screenshots
![COVID-19 Tracker Screenshot](../readme-assets/pictures/COVID-19-Tracker.png)
![COVID-19 Tracker Screenshot](../readme-assets/pictures/COVID-19-Tracker-2.png)

## Motivation 
> The motivation for this project came from the inability for people to access accurate, up to date, unbiased, and easily digestible information. There's a lot of misinformation regarding this pandemic and this is a tool to counter that, providing the raw unbaised numbers without having to navigate through government websites. Many COVID-19 trackers have hard to read charts or tables and there's rarely any maps to digest and understand the data. Some maps only show certain countries and it's important to show information from the entire world as this is a worldwide pandemic. Many maps don't show the individual data points, instead clustering the data from each province or state. 

## Technologies
#### ReactJS
> [ReactJS](https://reactjs.org/) is the web framework for this project. It's used due to its ease of creating front end components quickly with minimal code and its efficient updating and rendering.
[React GitHub](https://github.com/facebook/react)

#### Deck.gl
> [Deck.gl](https://deck.gl/) is used for powerful and efficient web data visualizations. Deck.gl is used for creating the scatterplot layer and the heatmap layer which are essential aspects of this project. It's able to handle 2500+ COVID-19 data points with no problems due to its efficiency and as it uses the reactive programming paradigm.
[Deck.gl GitHub](https://github.com/uber/deck.gl)

#### Google Maps API
> The [Google Maps JavaScript API](https://developers.google.com/maps/documentation/javascript/tutorial) is used as the base map for this project. Due to its flexibility a [custom Google Maps react component](../master/src/components/Map.js) was created. The Google Maps API can be accessed using the [Google Developers Console](https://console.developers.google.com/), API keys are required for this project.

#### Firebase
> [Firebase](https://firebase.google.com/) is used for the hosting and deployment of this project. Firebase provides powerful features such as analytics and its cloud functions. It's also easily scalable.

#### Data Source
> The data source comes from the [Coronavirus Tracker API](https://github.com/ExpDev07/coronavirus-tracker-api). Worldwide Data comes Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE) and US data comes from the Conference of State Bank Supervisors. The API provides up to date and accurate data with coordinates, 2500+ data points and more, making it a great source of COVID-19 data!

## Future Features
  * Recoveries are planned but not available yet to due [issues with the data source](https://github.com/ExpDev07/coronavirus-tracker-api/issues/161)
  * Additional accurate sources for more data points in Asia and Europe
  * Infected data parameter option: Takes confirmed cases and subtracts deaths and recoveries
  * Updated UI and homepage
  * Graphs to see if countries or states / provinces are "flattening the curve" 
    * Logarithmic scale graphs
  * Deck.gl Text layer with data clustering as the default layer option for mobile
  * Table with sorted data with each countries' cases, deaths and recoveries
  * Data History and timeline
  * Machine Learning Predictions


## Getting Started
* Clone or fork this repository.
```
git clone
```

* Install all dependencies with [npm](https://nodejs.org/)
```
npm install
```

* Get your Google Maps API key from the [Google Developers Console](https://console.developers.google.com/) and put it in a `.env` file.
```
REACT_APP_GOOGLE_API_KEY = <your API key>
```

* Run the project
```
npm start
```

## Contributions
> If you're new to open source contributions read [this guide](https://opensource.guide/how-to-contribute/). Issues and pull requests are welcome!
