# Hypervideo-Card
Card plugin for [Hypervideos.js](https://github.com/Aleix88/Hypervideos)
<div>
    <img src="https://github.com/Aleix88/Hypervideo-Card/blob/main/card.png?raw=true">
</div>

## Features
- Display a modal card with an image, title, description and an href button(optional).
- Customize all the background colors, text colors and images.

## Installation
### Manual downloading
1. Download the Card.js file.
2. Import this file in your html.

## Usage
Add this plugin to the hypervideo configuration object with the text paràmeter on config:

    const config = {
        ...

        "tags": [
          {
            ...

            "plugin": {
                "name": "Card",
                "config": {
                    "title": "Modal title",
                    "description": "Modal description",
                    "imageSrc": "image.jpg",
                    "backgroundColor": "#F2D5A0",
                    "titleColor": "rgb(138 104 43)",
                    "descriptionColor": "rgb(138 104 43)",
                    "button": {
                      "title": "Button text",
                      "href": "https://www.google.com", 
                      "backgroundColor": "rgb(138 104 43)",
                      "textColor": "white"
                    }
                }
            }

          }, 
          ...
        ]
      };

## Config parameters

| Field | Type | Description |
| ------------- | ------------- | ------------- |
| title | string | Modal title |
| description | string | Modal description |
| imageSrc | string | Path of the image |
| backgroundColor | string | Modal background color. Any color format accepted in css. |
| titleColor | string | Modal title color. Any color format accepted in css. |
| descriptionColor | string | Modal description color. Any color format accepted in css. |
| button (optional) | object | Configuration of the link button. Contains the following fields:<br/>- title (string) - Button text<br/>- href (string) - Link to open on click.<br/>- backgroundColor (string) - Button background color.<br/>- textColor (string) - Button text color |