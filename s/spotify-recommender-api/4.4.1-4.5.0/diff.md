# Comparing `tmp/spotify_recommender_api-4.4.1-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-4.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 41854 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       21 b- defN 23-Jul-01 20:09 spotify_recommender_api/__init__.py
+Zip file size: 42685 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       21 b- defN 23-Jul-01 23:53 spotify_recommender_api/__init__.py
 -rw-rw-r--  2.0 unx     1263 b- defN 23-Jul-01 13:50 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    15410 b- defN 23-Jul-01 20:09 spotify_recommender_api/core.py
--rw-rw-r--  2.0 unx     2042 b- defN 23-Jun-23 14:32 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx   116945 b- defN 23-Jul-01 20:10 spotify_recommender_api/recommender.py
--rw-rw-r--  2.0 unx     6306 b- defN 23-Jul-01 13:51 spotify_recommender_api/request_handler.py
+-rw-rw-r--  2.0 unx    15896 b- defN 23-Jul-01 23:53 spotify_recommender_api/core.py
+-rw-rw-r--  2.0 unx     2042 b- defN 23-Jul-01 23:52 spotify_recommender_api/error.py
+-rw-rw-r--  2.0 unx   121606 b- defN 23-Jul-02 00:01 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx     6217 b- defN 23-Jul-01 23:52 spotify_recommender_api/request_handler.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
 -rw-rw-r--  2.0 unx     6722 b- defN 23-Jul-01 13:51 spotify_recommender_api/server.py
--rw-rw-r--  2.0 unx     9726 b- defN 23-Jul-01 20:09 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    21574 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-01 20:11 spotify_recommender_api-4.4.1.dist-info/RECORD
-13 files, 181418 bytes uncompressed, 39822 bytes compressed:  78.0%
+-rw-rw-r--  2.0 unx     9757 b- defN 23-Jul-01 23:53 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx    22073 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Jul-02 00:02 spotify_recommender_api-4.5.0.dist-info/RECORD
+13 files, 187006 bytes uncompressed, 40653 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: spotify_recommender_api/server.py
 Comment: 
 
 Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api-4.4.1.dist-info/METADATA
+Filename: spotify_recommender_api-4.5.0.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-4.4.1.dist-info/WHEEL
+Filename: spotify_recommender_api-4.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-4.4.1.dist-info/top_level.txt
+Filename: spotify_recommender_api-4.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-4.4.1.dist-info/RECORD
+Filename: spotify_recommender_api-4.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '4.4.1'
+__version__ = '4.5.0'
```

## spotify_recommender_api/core.py

```diff
@@ -152,15 +152,15 @@
     if type == 'song':
         playlist_name = f"{additional_info!r} Related"
         description = f"Songs related to {additional_info!r}, within the playlist {base_playlist_name}"
     elif type in {'short', 'medium'}:
         playlist_name = "Recent-ish Favorites" if type == 'medium' else "Latest Favorites"
         description = f"Songs related to your {type} term top 5, within the playlist {base_playlist_name}"
 
-    elif 'most-listened' in type:
+    elif 'most-listened' in type and 'recommendation' not in type:
         playlist_name = f"{type.replace('most-listened-', '').capitalize()} Term Most-listened Tracks"
         description = f"The most listened tracks in a {type.replace('most-listened-', '')} period of time"
 
     elif type == 'artist-related':
         playlist_name = f"{additional_info!r} Mix"
         description = f"Songs related to {additional_info!r}, within the playlist {base_playlist_name}"
 
@@ -201,25 +201,39 @@
         playlist_name = f"General Recommendation based on {additional_info[1]}"
         description = additional_info[0]
 
     elif type == 'mood':
         playlist_name = f"{additional_info[0]} Songs".capitalize()
         description = f'Songs related to the mood "{additional_info[0]}"{", excluding the mostly instrumental songs" if additional_info[1] else ""}, within the playlist {base_playlist_name}'
 
+    elif type == 'most-listened-recommendation':
+        playlist_name = f"{additional_info.replace('_', ' ')} most listened recommendations".capitalize() # type: ignore
+        description = f"Songs related to the {additional_info.replace('_', ' ')} most listened tracks, within the playlist {base_playlist_name}" # type: ignore
+
     else:
         raise ValueError('type not valid')
 
     if playlist_found := util.playlist_exists(name=playlist_name, base_playlist_name=base_playlist_name, headers=headers, _update_created_playlists=_update_created_playlists):
         new_id = playlist_found[0]
 
-        playlist_tracks = list(map(lambda track: {'uri': track['track']['uri']}, requests.get_request(
-            url=f'https://api.spotify.com/v1/playlists/{new_id}/tracks', headers=headers).json()['items']))
+        playlist_tracks = [
+            {
+                'uri': track['track']['uri']
+            }
+            for track in requests.get_request(
+                headers=headers,
+                url=f'https://api.spotify.com/v1/playlists/{new_id}/tracks',
+            ).json()['items']
+        ]
 
         delete_json = requests.delete_request(
-            url=f'https://api.spotify.com/v1/playlists/{new_id}/tracks', headers=headers, data={"tracks": playlist_tracks}).json()
+            headers=headers,
+            data={"tracks": playlist_tracks},
+            url=f'https://api.spotify.com/v1/playlists/{new_id}/tracks',
+        ).json()
 
         if (
             _update_created_playlists or
             (
                 playlist_name.lower().startswith('short term profile recommendation') and
                 playlist_found[1] == playlist_name.replace('Short term ', '')
             )
@@ -236,14 +250,15 @@
 
     else:
         data = {
             "name": playlist_name,
             "description": description,
             "public": False
         }
+
         playlist_creation = requests.post_request(url=f'https://api.spotify.com/v1/users/{user_id}/playlists', headers=headers, data=data)
         new_id = playlist_creation.json()['id']
 
     return new_id
 
 
 def create_playlist_data_dict(row) -> dict:
```

## spotify_recommender_api/recommender.py

```diff
@@ -72,22 +72,21 @@
         return True
 
     def __get_song_genres(self, song: 'dict[str, Any]') -> 'list[str]':
         """
         Function that gets all the genres for a given song
 
         Args:
-          song(dict[str,]): the song dictionary
+          song(dict[str, Any]): the song dictionary
 
         Returns:
           list[str]: list of genres for a given song
         """
         genres = []
-        song_artists = song["track"]["artists"] if 'track' in list(
-            song.keys()) else song["artists"]
+        song_artists = song["track"]["artists"] if 'track' in list(song.keys()) else song["artists"]
         for artist in song_artists:
             artist_id = artist["id"]
             if artist_id not in self.__artists:
                 artist_genres_res = requests.get_request(url=f'https://api.spotify.com/v1/artists/{artist_id}', headers=self.__headers)
                 try:
                     artist_genres = artist_genres_res.json()["genres"]
                     genres += artist_genres
@@ -114,16 +113,15 @@
             for offset in range(0, total_song_count, 100):
                 logging.info(f'Songs mapped: {offset}/{total_song_count}')
                 all_genres_res = requests.get_request(
                     headers=self.__headers,
                     url=f'https://api.spotify.com/v1/playlists/{self.__playlist_id}/tracks?limit=100&{offset=!s}'
                 )
                 for song in all_genres_res.json()["items"]:
-                    (id, name, popularity, artist, added_at), song_genres = util.song_data(
-                        song=song), self.__get_song_genres(song)
+                    (id, name, popularity, artist, added_at), song_genres = util.song_data(song=song), self.__get_song_genres(song)
                     song['id'] = id
                     danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
                     self.__songs.append({
                         "id": id,
                         "name": name,
                         "artists": artist,
                         "popularity": popularity,
@@ -426,15 +424,15 @@
 
         Raises:
             ValueError: Playlist does not contain the song
 
         Returns:
             int: the index for the song
         """
-        if song not in list(self.__playlist['name']):
+        if song not in self.__playlist['name'].tolist():
             raise ValueError(f'Playlist does not contain the song {song!r}')
 
         item = self.__playlist.index[self.__playlist['name'] == song].tolist()
 
         return item[0]
 
 
@@ -489,14 +487,15 @@
                 getattr(self, '_SpotifyAPI__playlist_recommendation_date', None),
                 getattr(self, '_SpotifyAPI__playlist_recommendation_time_range', None)
             ],
             'general-recommendation': [
                 getattr(self, '_SpotifyAPI__general_recommendation_description', None),
                 getattr(self, '_SpotifyAPI__general_recommendation_description_types', None)
             ],
+            'most-listened-recommendation': getattr(self, '_SpotifyAPI__most_listened_recommendation_time_range', None),
         }
 
 
         playlist_id = core.create_playlist(
             type=type,
             headers=self.__headers,
             user_id=self.__user_id,
@@ -696,15 +695,15 @@
 
         Returns:
             pd.DataFrame: song DataFrame
         """
         index = 0
         if type == 'song':
             index = self.__get_index_for_song(info)
-        elif type in {'medium', 'short', 'artist-related'}:
+        elif type in {'long', 'medium', 'short', 'artist-related'}:
             index = len(info) - 1
         else:
             raise ValueError('Type does not correspond to a valid option')
         song_dict = self.__song_dict if type == 'song' else info
         neighbors = self.__get_neighbors(song=index, K=K, song_dict=song_dict, type=type)
         return self.__song_list_to_df(neighbors, song_dict=song_dict)
 
@@ -763,41 +762,38 @@
         Args:
             time_range (str, optional): The time range to get the top 5 songs from ('medium', 'short'). Defaults to 'medium'.
 
         Raises:
             ValueError: time_range must be either medium_term or short_term
 
         Returns:
-            list[dict[str,]]: top 5 songs listened
+            list[dict[str, Any]]: top 5 songs listened
         """
         if time_range not in ['medium', 'short']:
-            raise ValueError(
-                'time_range must be either medium_term or short_term')
-        top_5 = requests.get_request(
-            url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit=5', headers=self.__headers).json()
+            raise ValueError('time_range must be either medium_term or short_term')
+
+        top_5 = requests.get_request(url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit=5', headers=self.__headers).json()
 
-        return list(
-            map(lambda song: {
+        return [
+            {
                 'name': song['name'],
                 'genres': self.__get_song_genres(song),
-                'artists': list(
-                    map(lambda artist: artist['name'], song['artists'])
-                ),
+                'artists': [artist['name'] for artist in song['artists']],
                 'popularity': song['popularity'],
-                'danceability': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'danceability'],
-                'loudness': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'loudness'],
-                'energy': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'energy'],
-                'instrumentalness': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'instrumentalness'],
-                'tempo': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'tempo'],
-                'valence': self.__playlist.drop_duplicates('id').loc[self.__playlist.drop_duplicates('id')['id'] == song['id'], 'valence']
-            }, list(
-                filter(lambda song: song['name'] in list(
-                    self.__playlist['name']), top_5['items'])
-            ))
-        )
+                'danceability': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['danceability'],
+                'loudness': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['loudness'],
+                'energy': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['energy'],
+                'instrumentalness': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['instrumentalness'],
+                'tempo': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['tempo'],
+                'valence': self.__playlist.drop_duplicates('id').query('id == @song["id"]')['valence']
+            }
+            for song in top_5['items']
+            if song['name'] in self.__playlist['name'].tolist()
+        ]
+
 
     def __find_recommendations_to_songs(self, base_songs: 'list[dict[str, Any]]', subset_name: str) -> 'dict[str, Any]':
         """Generates a song format record from a list of songs, with all the information the "song-based" recommendation needs
 
         Args:
             base_songs (list[dict[str, Any]]): List of base songs
             subset_name (str): Name of thihs subset of songs (barely seen, unless the dataframe is printed with this record in it)
@@ -1061,14 +1057,17 @@
 
             elif 'Playlist Recommendation' in name and ' - 20' not in name and 'playlist-recommendation' in playlist_types_to_update:
                 return True
 
             elif 'Songs related to the mood' in description and 'mood' in playlist_types_to_update:
                 return True
 
+            elif 'most listened recommendations' in name and 'most-listened-recommendation' in playlist_types_to_update:
+                return True
+
         return False
 
     def update_all_generated_playlists(
             self, *,
             K: Union[int, None] = None,
             playlist_types_to_update: Union['list[str]', None] = None,
             playlist_types_not_to_update: Union['list[str]', None] = None
@@ -1076,19 +1075,19 @@
         """Update all package generated playlists in batch
 
         Note:
             It is NOT recommended to use the K parameter in this function, unless 100% on purpose, since it will make all the playlists have the same number of songs in them
 
         Arguments:
             K (int, optional): Number of songs in the new playlists, if not set, defaults to the number of songs already in the playlist. Defaults to None.
-            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all == ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood'].
+            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all == ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood', 'most-listened-recommendation'].
             playlist_types_not_to_update (list[str], optional): List of playlist types not to update. For example, if you want to update all playlists but song-related playlists use this argument as ['song-related']. it can be used alongside with the playlist_types_to_update but it can become confusing or redundant. Defaults to none == [].
         """
         if playlist_types_to_update is None:
-            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood']
+            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation', 'mood', 'most-listened-recommendation']
 
         if playlist_types_not_to_update is None:
             playlist_types_not_to_update = []
 
         playlist_types_to_update = [playlist_type for playlist_type in playlist_types_to_update if playlist_type not in playlist_types_not_to_update]
 
         if 'profile-recommendation' in playlist_types_to_update:
@@ -1193,14 +1192,23 @@
                         self.get_songs_by_mood(
                             mood=mood,
                             K=total_tracks,
                             build_playlist=True,
                             exclude_mostly_instrumental=exclude_mostly_instrumental,
                         )
 
+                    elif 'most listened recommendations' in name and 'most-listened-recommendation' in playlist_types_to_update:
+                        time_range = '_'.join(name.split(' ')[:2]).lower()
+
+                        self.playlist_songs_based_on_most_listened_tracks(
+                            K=total_tracks,
+                            build_playlist=True,
+                            time_range=time_range,
+                        )
+
                 elif (
                     ' - 20' not in name and
                     'Profile Recommendation' in name and
                     any(
                         playlist_type in playlist_types_to_update
                         for playlist_type in {'short-term-profile-recommendation', 'medium-term-profile-recommendation', 'long-term-profile-recommendation'}
                     )
@@ -1255,55 +1263,50 @@
             ValueError: If the time_range parameter is not valid the error is raised.
             ValueError: If plot_top parameter is not valid the error is raised.
 
         Returns:
             pd.DataFrame: The dictionary that contains how many times each genre was spotted in the playlist in the given time range.
         """
         if time_range not in ['all_time', 'month', 'trimester', 'semester', 'year']:
-            raise ValueError(
-                'time_range must be one of the following: "all_time", "month", "trimester", "semester", "year"')
+            raise ValueError('time_range must be one of the following: "all_time", "month", "trimester", "semester", "year"')
 
         if plot_top and plot_top > 30:
-            raise ValueError(
-                'plot_top must be either an int smaller than 30 or False')
+            raise ValueError('plot_top must be either an int smaller than 30 or False')
 
-        playlist = self.__playlist[self.__playlist['added_at'] >
-                                   util.get_datetime_by_time_range(time_range=time_range)]
+        playlist = self.__playlist[self.__playlist['added_at'] > util.get_datetime_by_time_range(time_range=time_range)]
 
         if not len(playlist):
             logging.warning(f"No songs added to the playlist in the time range {time_range} ")
             return None
 
-        genres = list(reduce(lambda x, y: list(
-            x) + list(y), playlist['genres'], []))
+        genres = list(reduce(lambda x, y: list(x) + list(y), playlist['genres'], []))
 
-        genres_dict = dict(
-            reduce(lambda x, y: util.list_to_count_dict(dictionary=x, item=y), genres, {}))
+        genres_dict = dict(reduce(lambda x, y: util.list_to_count_dict(dictionary=x, item=y), genres, {}))
 
         genres_dict['total'] = len(playlist['genres'])
 
-        genres_dict = dict(
-            sorted(genres_dict.items(), key=lambda x: x[1], reverse=True))
+        genres_dict = dict(sorted(genres_dict.items(), key=lambda x: x[1], reverse=True))
 
-        genres_dict = util.value_dict_to_value_and_percentage_dict(
-            dictionary=genres_dict)
+        genres_dict = util.value_dict_to_value_and_percentage_dict(dictionary=genres_dict)
 
         dictionary = {'name': [], 'number of songs': [], 'rate': []}
 
         for key, value in genres_dict.items():
             dictionary['name'].append(key)
             dictionary['number of songs'].append(value['value'])
             dictionary['rate'].append(value['percentage'])
 
-        df = pd.DataFrame(data=dictionary, columns=[
-                          'name', 'number of songs', 'rate'])
+        df = pd.DataFrame(data=dictionary, columns=['name', 'number of songs', 'rate'])
 
         if plot_top:
-            core.plot_bar_chart(df=df, top=plot_top, plot_max=reduce(
-                lambda x, y: x + y, df['rate'][1:4], 0) >= 0.50)
+            core.plot_bar_chart(
+                df=df,
+                top=plot_top,
+                plot_max=reduce(lambda x, y: x + y, df['rate'][1:4], 0) >= 0.50
+            )
 
         return df
 
     def get_playlist_trending_artists(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> Union[pd.DataFrame, None]:
         """Calculates the amount of times each artist was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
@@ -1327,16 +1330,15 @@
         playlist = self.__playlist[self.__playlist['added_at'] >
                                    util.get_datetime_by_time_range(time_range=time_range)]
 
         if not len(playlist):
             logging.warning(f"No songs added to the playlist in the time range {time_range} ")
             return None
 
-        artists = list(reduce(lambda x, y: list(
-            x) + list(y), playlist['artists'], []))
+        artists = list(reduce(lambda x, y: list(x) + list(y), playlist['artists'], []))
 
         artists_dict = dict(reduce(lambda x, y: util.list_to_count_dict(
             dictionary=x, item=y), artists, {}))
 
         artists_dict['total'] = len(playlist['artists'])
 
         artists_dict = dict(sorted(artists_dict.items(),
@@ -2381,14 +2383,104 @@
                     self.__headers['Authorization'] = f'Bearer {auth_token}'
                 else:
                     break
 
         return playlist
 
 
+    def playlist_songs_based_on_most_listened_tracks(
+            self,
+            K: int = 50,
+            build_playlist: bool = False,
+            time_range: str = 'short_term',
+        ) -> Union[pd.DataFrame, None]:
+        """Function to create a playlist with songs from the base playlist that are the closest to the user's most listened songs
+
+        Args:
+            K (int, optional): Number of songs. Defaults to 50.
+            build_playlist (bool, optional): Flag to create the playlist in the user's library. Defaults to False.
+            time_range (str, optional): String to identify which is the time range, could be one of the following: {'short_term', 'medium_term', 'long_term'}. Defaults to 'short_term'.
+
+        Raises:
+            ValueError: time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'
+
+        Returns:
+            Union[pd.DataFrame, None]: DataFrame that contains the information of all songs in the new playlist
+        """
+        if time_range not in {'short_term', 'medium_term', 'long_term'}:
+            raise ValueError("time_range needs to be one of the following: 'short_term', 'medium_term', 'long_term'")
+
+        for _ in range(2):
+            try:
+
+                top_50 = requests.get_request(url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}&limit=50', headers=self.__headers).json()
+
+                top_50 = [
+                    {
+                        'id': song['id'],
+                        'name': song['name'],
+                        'genres': self.__get_song_genres(song),
+                        'artists': [artist['name'] for artist in song['artists']],
+                        'popularity': song['popularity']
+                    }
+                    for song in top_50['items']
+                ]
+
+                for song in top_50:
+                    danceability, loudness, energy, instrumentalness, tempo, valence = util.query_audio_features(song=song, headers=self.__headers)
+
+                    song.update({ # not using **song because the id isnt needed
+                        'danceability': danceability,
+                        'loudness': loudness,
+                        'energy': energy,
+                        'instrumentalness': instrumentalness,
+                        'tempo': tempo,
+                        'valence': valence,
+                    })
+
+
+                most_listened_recommendation = {
+                    'id': "UNOFFICIAL_ID",
+                    'name': f"{time_range.replace('_', ' ').capitalize()} Most Listened",
+                    'genres': list(reduce(lambda acc, x: acc + x['genres'], top_50, [])),
+                    'artists': list(reduce(lambda acc, x: acc + x['artists'], top_50, [])),
+                    'popularity': int(round(reduce(lambda acc, song: acc + int(song['popularity']), top_50, 0) / len(top_50))),
+                    'genres_indexed': self.__get_genres([util.item_list_indexed(song['genres'], all_items=self.__all_genres) for song in top_50]),
+                    'artists_indexed': self.__get_artists([util.item_list_indexed(song['artists'], all_items=self.__all_artists) for song in top_50]),
+                }
+
+                for audio_feature in ['danceability', 'loudness', 'energy', 'instrumentalness', 'tempo', 'valence']:
+                    most_listened_recommendation[audio_feature] = float(reduce(lambda acc, song: acc + float(song[audio_feature]), top_50, 0) / len(top_50))
+
+                song_dict = [*self.__song_dict, most_listened_recommendation]
+
+                playlist = self.__get_recommendations(type=time_range.split('_')[0], info=song_dict, K=K)
+
+                if build_playlist:
+                    ids = playlist['id'].tolist()
+                    self.__most_listened_recommendation_time_range = time_range
+
+                    self.__write_playlist(
+                        K=K,
+                        type=f'most-listened-recommendation',
+                        additional_info=ids
+                    )
+
+                return playlist
+
+            except AccessTokenExpiredError as e:
+                logging.warning('Error due to the access token expiration')
+                auth_token = auth.get_auth()
+
+                self.__auth_token = auth_token
+
+                self.__headers['Authorization'] = f'Bearer {auth_token}'
+
+
+
 
 def start_api(user_id: str, *, playlist_url: Union[str, None] = None, playlist_id: Union[str, None] = None, liked_songs: bool = False, log_level: str = 'INFO', prepare_favorites: bool = False):
     """Function that prepares for and initializes the API
 
     Note:
         Internet Connection is required
```

## spotify_recommender_api/request_handler.py

```diff
@@ -36,15 +36,15 @@
             return response
         except Exception as e:
             if any(errorCode in f'{e}' for errorCode in ['404', '50']):
                 continue
 
             if '401' in f'{e}':
                 logging.error('Access Token Expired')
-                raise AccessTokenExpiredError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs) from e
+                raise AccessTokenExpiredError(func_name=func.__name__, message=None, *args, **kwargs) from e
 
             if '429' not in f'{e}':
                 raise HTTPRequestError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs) from e
 
             if x == 0:
                 logging.warning('\nExponential backoff triggered: ')
```

## spotify_recommender_api/util.py

```diff
@@ -91,15 +91,15 @@
         str|bool: If the playlist already exists, returns the id of the playlist, otherwise returns False
     """
     total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=1', headers=headers).json()['total']
     playlists = []
     for offset in range(0, total_playlist_count, 50):
         request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=headers).json()
 
-        playlists += list(map(lambda playlist: (playlist['id'], playlist['name'], playlist['description']), request['items']))
+        playlists += [(playlist['id'], playlist['name'], playlist['description']) for playlist in request['items']]
 
     return next(
         (
             playlist for playlist in playlists
             if (
                 playlist[1] == name or
                 (
@@ -115,19 +115,19 @@
             )
         ),
         ()
     )
 
 
 
-def query_audio_features(song: pd.Series, headers: dict) -> 'list[float]':
+def query_audio_features(song: Union[pd.Series, 'dict[str, Any]'], headers: dict) -> 'list[float]':
     """Queries the audio features for a given song and returns the ones that match the recommendations within this package
 
     Args:
-        song (pd.Series): song containing its base information
+        song (pd.Series | dict[str, Any]): song containing its base information
         headers (dict): Request headers
 
     Returns:
         list[float]: list with the audio features for the given song
     """
 
     song_id = song['id']
```

## Comparing `spotify_recommender_api-4.4.1.dist-info/METADATA` & `spotify_recommender_api-4.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 4.4.1
+Version: 4.5.0
 Summary: Python package which takes the songs of a greater playlist as starting point to make recommendations of groups of songs that might bond well within that same playlist, using K-Nearest-Neighbors Technique
 Home-page: https://github.com/nikolas-virionis/spotify-api
 Author: Nikolas B Virionis
 Author-email: nikolas.virionis@bandtec.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -265,14 +265,23 @@
 # Parameters
 get_songs_by_mood(mood: str, K: int = 50, build_playlist: bool = False, exclude_mostly_instrumental: bool = False)
 # Method Use Example
 api.get_songs_by_mood(mood='happy', build_playlist=True)
 # Function to create a playlist based on the general mood of its songs
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~~~~
+ - playlist_songs_based_on_most_listened_tracks
+~~~python
+# Parameters
+playlist_songs_based_on_most_listened_tracks(K: int = 50, build_playlist: bool = False, time_range: str = 'short_term')
+# Method Use Example
+api.playlist_songs_based_on_most_listened_tracks(time_range='medium_term', build_playlist=True)
+# Function to create a playlist with songs from the base playlist that are the closest to the user's most listened songs
+# BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
+~~~~~~
  - get_medium_term_favorites_playlist - DEPRECATED
 ~~~python
 # Parameters
 get_medium_term_favorites_playlist(with_distance: bool, generate_csv: bool,
                         generate_parquet: bool, build_playlist: bool)
 # Method Use Example
 api.get_medium_term_favorites_playlist(generate_csv=True, build_playlist=True)
```

## Comparing `spotify_recommender_api-4.4.1.dist-info/RECORD` & `spotify_recommender_api-4.5.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-spotify_recommender_api/__init__.py,sha256=jE7Hja-Saozkka8sEZeybOD8E6vMn9F1pXhgRC7q-YM,21
+spotify_recommender_api/__init__.py,sha256=a4qsqPKUrk6Ur9lXXKPt7KEI5zaqiA8s2bLsPUcPw9s,21
 spotify_recommender_api/authentication.py,sha256=jQ49ZXeZ9Vj6x76aooA7uQ09xRRETmMDYCfeRw0TaPQ,1263
-spotify_recommender_api/core.py,sha256=e33Q3Cs_Q-jUcjRzGJRIOIG7YQTVPtWZOzdn19wGikw,15410
+spotify_recommender_api/core.py,sha256=ri6BRqe6znUsacjZLPzcwE3kuH4H9-1M7uVPHPhdhbA,15896
 spotify_recommender_api/error.py,sha256=BBG5MUYuoAGElBAV058H6o13R-bYR_sGGgjAT1r7lCg,2042
-spotify_recommender_api/recommender.py,sha256=kGpSNiNbQA9PHoMbNDs4YYhtVzbFz9e1Z49IEdYsxAg,116945
-spotify_recommender_api/request_handler.py,sha256=f9aqL1s_Kjqvf5NUeDkvJfVC8xgEcLjBq61aO3wdmkk,6306
+spotify_recommender_api/recommender.py,sha256=K2rvp1j4cEQvYwW8iA4TbdZXNllgyD9-3ogoBkdoJKM,121606
+spotify_recommender_api/request_handler.py,sha256=uZabNApJIdnuUL_wN8KRKWRAwEDVjK0BB4QaG4SHjRM,6217
 spotify_recommender_api/sensitive.py,sha256=Xn2FFn4uUk94Ei_It1U2iT5ZZEafHBt9q--lSPwlaoI,99
 spotify_recommender_api/server.py,sha256=Jq90Sd6GrI4txMaLFDcNoThy3jSWe8MwVUIvQXSkkYQ,6722
-spotify_recommender_api/util.py,sha256=YKe6uhOml0kvsjt9ciXEpuRhPh4uZfi3uik9xzPvYaw,9726
-spotify_recommender_api-4.4.1.dist-info/METADATA,sha256=8eFHiOy52QO83p0rHuHiNadf6INestg6GAKfLf78OC4,21574
-spotify_recommender_api-4.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-spotify_recommender_api-4.4.1.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
-spotify_recommender_api-4.4.1.dist-info/RECORD,,
+spotify_recommender_api/util.py,sha256=n72S-Jsi7uu8Vvhy7ArgBTXRdSYO-FDo1lMksoVB4oM,9757
+spotify_recommender_api-4.5.0.dist-info/METADATA,sha256=X0f26shnWoXb0G4ebUD2jEijSwQihUApkJwB-ccLJEQ,22073
+spotify_recommender_api-4.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spotify_recommender_api-4.5.0.dist-info/top_level.txt,sha256=X65Ob3YNye88oWqQCXBvKpEUdmLQvio-wg4Ra2Gsh-c,24
+spotify_recommender_api-4.5.0.dist-info/RECORD,,
```

