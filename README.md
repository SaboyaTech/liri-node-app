# Terminal Liri Node App:

LIRI is like iPhone's SIRI, however, while SIRI is a Speech Interpretation and Recognition Interface, LIRI will be a command line node app that takes in parameters and gives you back data.

I have created a .env.example file, remane it to .env and place your API keys in it.

### Goals:

- To search Spotify for any song, OMDB for movies, and the Stock Market.
- To be retireve the data from the Data Bases, and to display the results on to the terminal.
- liri.js can take one of this commands
- **<em>spotify_this_song</em>**
- **<em>movie_this</em>**
- **<em>check_the_market</em>**
- **<em>do_what_it_says</em>**

### Required:

- Spotify API-Key
- OMDB API-Key
- Alpha Vantange API-Key

### Tools:

| Module           | Purpose                                                          |
| ---------------- | ---------------------------------------------------------------- |
| Axious           | To grab data from the OMDB API                                   |
| DotEnv           | Loads environment variables from .env file.                      |
| Node-Spotify-API | Allows to get access to the Spotify Database with Authentication |

### Set-Up:

```
liri-node-app$ npm install

liri-node-app$ mv .env.example/ .env/   // This will rename the Directory
```

### Commands:

- **spotify_this_song:** &nbsp; :arrow_right: &nbsp; `node liri.js spotify_this_song '<song search here>'`  
  <br>

  **Output:**

        * Artist(s)
        * Name of the song
        * A preview link of the song from Spotify
        * Name of Album

  <em>If no song is provided then your program will default to "The Sign" by Ace of Base.</em>
  <br>

  ![github](https://raw.githubusercontent.com/SaboyaDev/liri-node-app/master/GIFs/spotify-this-song-default-val.gif)

  ![github](https://raw.githubusercontent.com/SaboyaDev/liri-node-app/master/GIFs/spotify-this-song-any-song.gif)

---

2.  **movie_this:** &nbsp; :arrow_right: &nbsp; `node liri.js movie_this '<movie title here>'`
    <br>

    **Output:**

          * Title of the movie.
          * Year the movie came out.
          * IMDB Rating of the movie.
          * Rotten Tomatoes Rating of the movie.
          * Country where the movie was produced.
          * Language of the movie.
          * Plot of the movie.
          * Actors in the movie.

      <br>

    ![github](https://raw.githubusercontent.com/SaboyaDev/liri-node-app/master/GIFs/movie-this-default-value.gif)

    ![github](https://raw.githubusercontent.com/joseluissaboya/liri-node-app/master/GIFs/movie-this-any-movie.gif)

---

3.  **check_the_market:** &nbsp; :arrow_right: &nbsp; `node liri.js check_the_market '<stock symbol>'`
    <br>

    This will connect with the Alpha Vantage API which will provide us with the daily performance of any stock and display the following results:

      <br>
      
      **Output:**
      ```
        * Time Zone
        * The Symbol
        * The Opening Price
        * The closing Price
        * The High of the Day
        * The Low of the Day
        * The Closing Price
      ```

    ![github](https://raw.githubusercontent.com/joseluissaboya/liri-node-app/master/GIFs/check-the-market.gif)

---

4. **do_what_it_says:** &nbsp; :arrow_right: &nbsp; `node liri.js do_what_it_says`
   <br >

- Using the `fs` Node package, LIRI will take the text inside of random.txt and then use it to call one of LIRI's commands.

- It should run `spotify-this-song` for "I Want it That Way," as follows the text in `random.txt`.
  <br>
  ![github](https://raw.githubusercontent.com/joseluissaboya/liri-node-app/master/GIFs/read-file-do-task.gif)

---

SaboyaDev
