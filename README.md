<h1 align="center">
  Andy Brown - iOS Portfolio
</h1>

<p align="center">
    <a href="mailto:andybrown41@icloud.com">Email Me</a> ·
    <a href="https://github.com/ab492/iOS-Portfolio/blob/master/Andy%20Brown%20-%20iOS%20Developer%20-%20July%202019.pdf">Download CV</a>
</p>

# Skrilla

[Skrilla](https://github.com/ab492/Skrilla)  is a 'dummy' banking app exploring some of the elements of popular banking apps: biometric and keychain authentication; viewing transactions; assigning a category and receipt to a transaction; splitting a bill with friends and sharing the transaction with them.

I had great fun designing and building this app. A particular challenge was writing the 'Split Transaction' methods as I came across many issues I hadn't thought about previously: how do you split an odd amount of money between friends fairly?; how do you re-calculate the split when the user has assigned a custom amount for some of the friends? This forced me to return to the drawing board for large parts of my model code, in turn teaching me about the importance of keeping a clear separation of concerns between objects.

![](https://github.com/ab492/iOS-Portfolio/blob/master/PortfolioScreengrabs/Skrilla_Portfolio.png)


### Technologies Used
* Written fully in Swift.
* MVC app architecture.
* Persisting data and caching images.
* Using 3rd party libraries with CocoaPods.
* Writing and reading from the keychain (to store user defined password).
* Biometric authentication with FaceID/TouchID, depending on device.
* Separating data sources from view controllers.
* Custom protcols (SplitTransactionCellDelegate).
* Custom views (CategoryView).
* Extending classes to add custom functionality for my needs.
* Exporting and importing user data using UIActivityController.
* Using a linter to ensure consistent formatting through the project.

# Flip Flop Weather

[FlipFlopWeather](https://github.com/ab492/FlipFlopWeather) is a prototype weather app for flip flops lovers. You can add favourite locations, view the current weather and forecast in those locations, and get some support that it's 'flip flop weather' outside. You can also get notifications from your favourites, and view them on a map.

I'm really happy with the models I wrote for this app: everything has a clear task, separate from other objects, and I've worked hard to pass updates around my app using delegates, protocols and notifications.

![](https://github.com/ab492/iOS-Portfolio/blob/master/PortfolioScreengrabs/FlipFlopWeather_Portfolio.png)

### Technologies Used
* MVC and MVVM design patterns.
* Coordinator pattern to control the navigation flow of the app.
* Parsing JSON from OpenWeatherAPI and transforming it to fit the required model, along with persisting the data.
* Keeping a clear separation of concerns between classes (API managers, model controllers and carving datasources away from view controllers).
* Using 3rd party libraries with CocoaPods.
* Local notifications.
* MapKit and CoreLocation.
* Networking using URLSession, combined with completion handlers and GCD.
* Autolayout and stack views.
* Custom UIViews.
* Animation.
* Custom protcols (FavouritesModelControllerObserver to notify objects when the model updates).
* Custom views (TemperaturePreferenceButton).
* Extending classes to add custom functionality for my needs.
* Using a linter to ensure consistent formatting through the project.
* Using R.swift to get strong typed resources.
