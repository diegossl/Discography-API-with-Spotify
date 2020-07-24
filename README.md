# Musicfy API

The Musicfy API is an information collection tool using a Spotify web API. With it it is possible to extract information about artists and their discography.

## Setup

To execute the project, it will be necessary to install the dependencies by typing the following command in the terminal:

```bash
yarn install
```

Then create a file called **.env** and copy the contents of the file **.env.exemple** to it, which already exists at the root of the project. After that, fill in the fields with your credentials.

### Use

To execute the project, type the following command in the terminal:

```bash
yarn start
```

The system is now ready to be used via the routes:

[http://localhost:3000/artist/info](http://localhost:3000/artist/info)

[http://localhost:3000/artist/albums](http://localhost:3000/artist/albums)

Just send a request for these routes with a JSON containing the artist's name.

### Example of data entry:

```javascript
{
	"artistName": "Ivete Sangalo"
}
```
### Example output: Artist

```javascript
{
  "name": "Ivete Sangalo",
  "genres": [
    "axe",
    "baile pop",
    "mpb",
    "pagode",
    "pop nacional",
    "samba reggae"
  ],
  "popularity": 70,
  "spotifyPage": "spotify:artist:7dzq55YG3wjViqexDwiycQ"
}
```

### Example output: Albuns

```javascript
[
  {
    "name": "Arraiá Da Veveta",
    "releaseDate": "2020-06-21",
    "totalTracks": 9,
    "spotifyPage": "spotify:album:2uASdtYZsn2RljUVbYy8Ep"
  },
  {
    "name": "Ivete Sangalo Live Experience (Ao Vivo Em São Paulo / 2018)",
    "releaseDate": "2019-04-12",
    "totalTracks": 30,
    "spotifyPage": "spotify:album:0qO6ZPC8y2eXVA1AidKGZQ"
  },
  {
    "name": "Duetos 2",
    "releaseDate": "2017-11-24",
    "totalTracks": 16,
    "spotifyPage": "spotify:album:3uta1AqyOI8qoVUB6A8MTX"
  },
  {
    "name": "Acústico Em Trancoso (Ao Vivo)",
    "releaseDate": "2016-07-29",
    "totalTracks": 24,
    "spotifyPage": "spotify:album:6Aqv0T76VtYRBhZMsd0Pa4"
  },
  {
    "name": "O Carnaval De Ivete Sangalo - Sai Do Chão (Ao Vivo)",
    "releaseDate": "2015-12-11",
    "totalTracks": 18,
    "spotifyPage": "spotify:album:0ggbRn1mM1fojrFOGJl6lR"
  },
  {
    "name": "Viva Tim Maia",
    "releaseDate": "2015-07-31",
    "totalTracks": 12,
    "spotifyPage": "spotify:album:0s6eeWdtRBJjhWFjXG9Bcq"
  },
  {
    "name": "Multishow Ao Vivo - Ivete Sangalo 20 Anos (Live)",
    "releaseDate": "2014-05-06",
    "totalTracks": 18,
    "spotifyPage": "spotify:album:3BezFc7G2hTrTO9o7WX2D2"
  },
  {
    "name": "O Carnaval De Ivete Sangalo 2015 (Ao Vivo)",
    "releaseDate": "2014-01-01",
    "totalTracks": 18,
    "spotifyPage": "spotify:album:0BGtZFqDInZuJJvJa8jChx"
  },
  {
    "name": "As Nossas Canções",
    "releaseDate": "2013-01-01",
    "totalTracks": 16,
    "spotifyPage": "spotify:album:04TLo3kfhsjXttswMuBGbS"
  },
  {
    "name": "Real Fantasia (International Version)",
    "releaseDate": "2013-01-01",
    "totalTracks": 14,
    "spotifyPage": "spotify:album:3iPYe8UrC6vbnQAsNBtHr0"
  },
  {
    "name": "Especial Ivete Gil Caetano (Ao Vivo)",
    "releaseDate": "2012-05-14",
    "totalTracks": 15,
    "spotifyPage": "spotify:album:0fGDlwWo9GAfIRNAnOSxh6"
  },
  {
    "name": "Baladas de Ivete",
    "releaseDate": "2012-01-01",
    "totalTracks": 15,
    "spotifyPage": "spotify:album:1gcEnxHbhuUhNwo4JfIcJq"
  },
  {
    "name": "Especial Ivete, Gil E Caetano",
    "releaseDate": "2012-01-01",
    "totalTracks": 15,
    "spotifyPage": "spotify:album:3hOAYii7ltL7zatrSVtBQc"
  },
  {
    "name": "O Carnaval De Ivete Sangalo 2013 (Ao Vivo)",
    "releaseDate": "2012-01-01",
    "totalTracks": 16,
    "spotifyPage": "spotify:album:04BqrkFIIy6vkNHhkXC6qd"
  },
  {
    "name": "Real Fantasia (Deluxe Edition)",
    "releaseDate": "2012-01-01",
    "totalTracks": 15,
    "spotifyPage": "spotify:album:5wUaAeJiu6XDFpPhRnMegS"
  },
  {
    "name": "Real Fantasia",
    "releaseDate": "2012-01-01",
    "totalTracks": 14,
    "spotifyPage": "spotify:album:6jK2GfT9HRxmO9snF3iYMM"
  },
  {
    "name": "Multishow Ao Vivo - Ivete Sangalo No Madison Square Garden (Ao Vivo No Madison Square Garden / 2010)",
    "releaseDate": "2010-01-01",
    "totalTracks": 18,
    "spotifyPage": "spotify:album:2OzxcLL2uclyduNsqogqng"
  },
  {
    "name": "Multishow Registro Pode Entrar",
    "releaseDate": "2009",
    "totalTracks": 17,
    "spotifyPage": "spotify:album:34OckNIZ8nCUJRJ3zxxDu7"
  },
  {
    "name": "A Casa Amarela",
    "releaseDate": "2008-01-01",
    "totalTracks": 11,
    "spotifyPage": "spotify:album:0jywJRnZjCDN6faNkHUrrl"
  },
  {
    "name": "Ivete Sangalo Sem Limite",
    "releaseDate": "2007-01-08",
    "totalTracks": 27,
    "spotifyPage": "spotify:album:5fLXDLRiKLK9zFvLBlunzB"
  }
]
```

## License

MIT
