Instructions for Setting Up Google Maps API Key and Adding Locations
Obtain a Google Maps API Key:

Visit the Google Cloud Console.
Create a project or select an existing one.
Go to APIs & Services > Library.
Search for Maps JavaScript API and enable it.
Under APIs & Services > Credentials, click Create Credentials and select API key.
Copy the API key and replace YOUR_API_KEY in the script URL in the HTML code.
Add More Locations:

In the initMap function, add more markers by defining additional coordinates.
Example:
javascript
Copy code
new google.maps.Marker({
    position: { lat: 34.0522, lng: -118.2437 }, // Coordinates for Los Angeles, CA
    map: map,
    title: "Significant Location: Los Angeles, CA",
});
Repeat this code block for each additional location you’d like to mark on the map, updating the lat, lng, and title properties as needed.
Future Additions:

Each time you want to add a new location, simply add another google.maps.Marker section within the initMap function.
Update the title and coordinates accordingly to reflect each unique place associated with different milestones in the timeline.
