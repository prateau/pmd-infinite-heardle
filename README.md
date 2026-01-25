# :no_entry: [DEPRECATED] Active at https://github.com/prateau-heardle/pmd-heardle

# pkmn-md-infinite-heardle

A clone of [Heardle](https://www.heardle.app/), and [K-Pop Heardle](https://heardle-kpop.glitch.me/) which can be played infinitely and with Pokemon Mystery Dungeon's musics. Based on [Joywave Heardle](https://joywave-heardle.glitch.me/)

Each music is randomly chosen from Pokemon Mystery Dungeon's soundtrack album.

code edited from: [Pokemon infinite Heardle](https://pkmn-infinite-heardle.glitch.me/)
<br />
<br />
HOW TO MAKE YOUR OWN INFINITE HEARDLE (UDPATED on **2024-02-03**)

1. **Remix this project** to create your own copy of the code
2. **Rename the project** with the URL that you'd like to Heardle to live at, by going to **Settings > Edit Project Details**
3. Open the **index.html** file & replace **"Pokemon Mystery Dungeon"** with the artist/genre of your heardle. Make sure to **do this first**, if you update the main.js first, sometimes your link will still show Joywave even after you update everything.
4. In the **index.html** file, you can update the image that gets shared with your link by updating lines **19-29**. To make sure the images show up correctly when sharing to twitter, make sure to use different links for the 2 sections!

(Items 5-12 are all edits to the **main.js file**)

5. On line **2** of **main.js** file and update **artist** with the **artist/genre** of your heardle - This will update all the text boxes & titles where "Pokemon Mystery Dungeon" shows up
6. On line **3** of **main.js** file, update **twitter** with your own twitter or instagram handle - This will update the contact info and replace every instance of "joywavez"
7. On line **7** of **main.js**, "const **musicNameList**" is initialized. Replace the text with a list of song titles that you want to show up as options in your Heardle. It should follow the format **"Song | Artist".** Make sure each song is in quotes and has a comma after it
8. On line **332** of **main.js**, "const **musicListWithLinks**" is initialized. Here you'll have to replace the links with links to your songs. Only Soundcloud links at the moment. Each link will have to follow the following format:
   **`{ url: "<link>", answer: "Song | Artist" },`**

   Make sure to have **at least 10 songs** in your lists otherwise you'll run into issues with the search bar!

9. If you want to edit the text in the **info button** on the top left, around **line 5457** you can update the text that shows up there. Search for **"A clone of..."** to find the line easier
10. If you want to edit the text in the **heart button** next to the info button, around **line 5746** you can update the text that shows up there. Search for **"Have questions"** to find the line easier

<br /> 
<br />

Glitch auto saves your code, so your changes should be available as soon as the code is editted.
<br />

Heardle sometimes doesnt work in the "Open Preview Pane" option, so it's best view it in the "Preview in new window" option
<br />

**ARCHIVING YOUR HEARDLE**
<br />
If your heardle goes blank/shows an empty page once it runs out of songs and you'd like to disable your site without archiving your site, you can update the **index.html** with a few lines of html.
I have an example of how to do that on **line 4** [here](https://glitch.com/edit/#!/testerheardle?path=index.html%3A55%3A0) and you can preview it [here](https://testerheardle.glitch.me/)
<br />
<br />

Feel free to tweet/dm @joywavez on twitter if you have any issues/questions!
<br />
<br />

**KNOWN ISSUES**

- Sometimes when you share your link to twitter, the image you added doesnt show up, even if you've updated the image link. I think its a twitter issue and not a code issue.

- For some songs, the timer on the player goes to 9 seconds instead of 16, and skips in intervals of 1.5 seconds instead of 1, 2, 3.. seconds each time. <br/>
  ~~I'm not sure why it happens, but it has something to do with the soundcloud links, so if anyone has any insight into why that happens, let me know!~~ <br/>

  Thanks to [archvile_drs](https://twitter.com/archvile_drs) on twitter for pointing out that this only seems to happen to songs in the first week of the Heardle.

- This code is specific to Soundcloud links.

  - I have a [youtube](https://glitch.com/~youtube-heardle-template) version, but its very basic and may have bugs; youtube links can be weird depending on your location, so it messes things up.

  - If you want to use a Spotify playlist, visit [https://audial.mogdan.xyz/custom](https://audial.mogdan.xyz/custom). You'll be able to add a link to your playlist and it seems to work similarly to Heardle.
