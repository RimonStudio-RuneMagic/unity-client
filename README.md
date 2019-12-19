# Rune Magic Javascript client
Client library to start using Rune Magic with Unity

Example Scene is provided.

## Installation
Download the latest unity package from [releases](/releases/latest) and import to your project.

After downloading insert the RuneMagicManager prefab to your scene, and fill the Token field with your token.

The package includes SocketIO library from https://assetstore.unity.com/packages/tools/network/socket-io-for-unity-21721 .


## Usage
For very simple usage example see `Examples/ExampleScript.cs` inside the package.

The class `RuneMagic` (from the namespace `RuneMagic`) have 4 static callbacks for listening to Rune events. 

`OnUpdate` is called every time a Rune sends information, with `JSONObject` param.
To read more about Rune data see [runes data documentation](https://github.com/RimonStudio-RuneMagic/runes-data).

`OnConnection` and `OnDisconnect` are called when the underlying socket connects or disconnected.

`OnError` is called on every error with connection or the usage, with an `object` param providing more details.



## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## License
[MIT](https://choosealicense.com/licenses/mit/) 