### Torrent API

#### Get latest torrents
* path: `/api/torrent/latest`
* method: `GET`
* return:
```javascript
{
	"page_count": <number>,
	"torrents": <Array>
}
```

#### Get specified torrent page
* path: `/api/torrent/page/:pagenum`
* method: `GET`
* params:
  * pagenum: <number>
* return:
```javascript
{
	"torrent": <Array>
}
```

#### Get torrents published by self
* path: `/api/torrent/my`
* method: `GET`
* return:
```javascript
{
	"page_count": <number>,
	"torrents": <Array>
}
```
* note:
  * user session required.

#### Get torrents published by team
* path: `/api/torrent/team`
* method: `GET`
* return:
```javascript
(TODO)
```

#### Search torrent by tag_id
* path: `/api/torrent/search`
* methid: `POST`
* post:
```javascript
{
	tag_id: <string>|<Array>
}
```
* return:
```javascript
(TODO)
```