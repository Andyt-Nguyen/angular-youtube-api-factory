**angular-youtube-api-factory** is an angularjs module with a youtube api factory.

* Author: Jonathan Hornung ([JohnnyTheTank](https://github.com/JohnnyTheTank))

## Usage

1. Install via [bower](http://bower.io/) :
    1. `bower install --save angular-youtube-api-factory`
2. Add `jtt_youtube` to your application's module dependencies.
3. Include dependencies in your HTML.
    1. When using bower:

        ```html
	    <script src="bower_components/angular/angular.js"></script>
	    <script src="bower_components/angular-youtube-api-factory/angular-youtube-api-factory.js"></script>
        ```

4. Use the factory `youtubeFactory`.


### factory functions

#### getVideos


```js
youtubeFactory.getVideosFromChannelById({
    channelId: <CHANNEL_ID>,
    order: <ORDER-TYPE>, // (optional) default: 'date'
    q: <SEARCH_STRING>, // (optional) filters the channel result with your search string (=q)
    maxResults: <MAX_RESULTS>, // (optional) default: 20
    key: key: <YOUR_API_KEY>,
});
```
```js
youtubeFactory.getVideosFromSearchByString({
    channelId: <CHANNEL_ID>,
    q: <SEARCH_STRING>, //optional, filters the channel result with your search string (=q)
    maxResults: <MAX_RESULTS>, // (optional) default: 20
    key: key: <YOUR_API_KEY>,
});
```

```js
youtubeFactory.getVideosFromPlaylistById({
    playlistId: <PLAYLIST_ID>,
    maxResults: <MAX_RESULTS>, // (optional) default: 20
    key: key: <YOUR_API_KEY>,
});
```


#### getChannel
```js
youtubeFactory.getChannelById({
    channelId: <CHANNEL_ID>,
    maxResults: <MAX_RESULTS>, // (optional) default: 1
    key: key: <YOUR_API_KEY>,
});
```


## Youtube JSON API

* Doku: https://developers.google.com/youtube/v3/docs/
* Api Explorer: https://developers.google.com/apis-explorer/#p/youtube/v3/
* Kanal-ID Converter: http://kid.yt.j.pfweb.eu/



[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/JohnnyTheTank/angular-youtube-api-factory/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

