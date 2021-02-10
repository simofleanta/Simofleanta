# Hello Friends! <img src="https://user-images.githubusercontent.com/1303154/88677602-1635ba80-d120-11ea-84d8-d263ba5fc3c0.gif" width="28px" alt="hi">

[![LinkedIn Connect](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/simonafleanta)
[![Instagram Follow](https://img.shields.io/badge/Instagram-Follow-green)](https://www.instagram.com/simo_fleanta/?hl=en)


#  What I do


```pyhon
   def me():
      return ...
```


- 🔭 I harness data to enable you to guide product innovation and business growth @Hirsch BI Solutions
- :computer: Most used packages in Python used : `Pandas, Seaborn, Matplotlib`
- 🤔 I’m looking for friends to go hiking, sharing ideas, working on open source projects.
- 😄 Pronouns: BI Analyst, Business Analyst.



# Profession

- :paperclip: [My Resume](https://github.com/simofleanta/Draft-Notebooks/files/5838026/Simona.Fleanta.Resume.pdf)
- :email: simo.fleanta@gmail.com



# My stack


<img align="left" alt="Visual Studio Code" width="26px" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/visual-studio-code/visual-studio-code.png" />

<img align="left" alt="Simofleanta | Jupyter" width="22px" color="#F2C811" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/jupyter.svg" />

<img align="left" alt="Simofleanta | mysql" width="22px" color="#F2C811" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/mysql.svg" />

<img align="left" alt="Simofleanta | python" width="22px" color="#F2C811" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/python.svg" />

<img align="left" alt="GitHub" width="26px" src="https://raw.githubusercontent.com/github/explore/78df643247d429f6cc873026c0622819ad797942/topics/github/github.png" />

<img align="left" alt="Simofleanta | Power BI" width="22px" color="#F2C811" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/powerbi.svg" />

<img align="left" alt="Simofleanta | Adobe Photoshop" width="22px" color="#F2C811" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/adobephotoshop.svg" />

<img align="left" alt="Simofleanta | Tableau" width="22px" color="#F2C811" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/tableau.svg" />

<br/>
<br/>




### Favorite Projects

- Domestic electricity analysis [Energy_Analysis](https://github.com/Hirsch-BI-Solutions/Electric-Energy-Consumption-Analysis)
- Ferntech Berlin [Ferntech](https://github.com/Hirsch-BI-Solutions/Ferntech-Insights/blob/main/Power%20%20Venture%20BI%20dashboard%20visual.MD)
- Konrad Adenauer Economic Policy [KAS](https://github.com/Tracking-International-Affairs/Economic-Policy-debate)
- BA Jobs report [BA Jobs](https://github.com/simofleanta/BA-Jobs-Report)
- Bertelsmann Scholarship Exercise [Udacity](https://github.com/simofleanta/Udacity)



#  Top languages

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=simofleanta)](https://github.com/Simofleanta/github-readme-stats)




# Activity

![Simo's github stats](https://github-readme-stats.vercel.app/api?username=simofleanta&show_icons=true&hide_border=true)

</details>

<br />
<br />

---
                                                                    


# Funk

[<img src="https://now-playing-simofleanta.vercel.app/api/spotify-playing" alt="simofleanta Spotify Playing" width="350" />](https://open.spotify.com/user/40ghawdoblwzgun5xf6ci4icm)


########################################################################################################################################



## Spotify

* Create a [Spotify Application](https://developer.spotify.com/dashboard/applications)
* Take note of:
    * `Client ID`
    * `Client Secret`
* Click on **Edit Settings**
* In **Redirect URIs**:
    * Add `http://localhost/callback/`

## Refresh Token

* Navigate to the following URL:

```
https://accounts.spotify.com/authorize?client_id={dee888fb4dee406fbc1776777c7f9853}&response_type=code&scope=user-read-currently-playing,user-read-recently-played&redirect_uri=http://localhost/callback/
```

* After logging in, save the {CODE} portion of: `http://localhost/callback/?code={CODE}`

* Create a string combining `{SPOTIFY_CLIENT_ID}:{SPOTIFY_CLIENT_SECRET}` (e.g. `5n7o4v5a3t7o5r2e3m1:5a8n7d3r4e2w5n8o2v3a7c5`) and **encode** into [Base64](https://base64.io/).

* Then run a [curl command](https://httpie.org/run) in the form of:
```sh
curl -X POST -H "Content-Type: application/x-www-form-urlencoded" -H "Authorization: Basic {BASE64}" -d "grant_type=authorization_code&redirect_uri=http://localhost/callback/&code={CODE}" https://accounts.spotify.com/api/token
```

* Save the Refresh token

## Vercel

* Register on [Vercel](https://vercel.com/)

* Fork this repo, then create a vercel project linked to it

* Add Environment Variables:
    * `https://vercel.com/<YourName>/<ProjectName>/settings/environment-variables`
        * `SPOTIFY_REFRESH_TOKEN`
        * `SPOTIFY_CLIENT_ID`
        * `SPOTIFY_SECRET_ID`

* Deploy!

## ReadMe

You can now use the following in your readme:

```[![Spotify](https://USER_NAME.vercel.app/api/spotify)](https://open.spotify.com/user/USER_NAME)```

## Customization

If you want a distinction between the widget showing your currently playing, and your recently playing:

### Hide the EQ bar

Remove the `#` in front of `contentBar` in [line 81](https://github.com/novatorem/novatorem/blob/98ba4a8489ad86f5f73e95088e620e8859d28e71/api/spotify.py#L81) of current master, then the EQ bar will be hidden when you're in not currently playing anything.

### Status String

Have a string saying either "Vibing to:" or "Last seen playing:".

* Change [`height` to `height + 40`](https://github.com/novatorem/novatorem/blob/5194a689253ee4c89a9d365260d6050923d93dd5/api/templates/spotify.html.j2#L1-L2) (or whatever `margin-top` is set to)
* Uncomment [**.main**'s `margin-top`](https://github.com/novatorem/novatorem/blob/5194a689253ee4c89a9d365260d6050923d93dd5/api/templates/spotify.html.j2#L10)
* Uncomment [currentStatus](https://github.com/novatorem/novatorem/blob/5194a689253ee4c89a9d365260d6050923d93dd5/api/templates/spotify.html.j2#L93)

## Requests

Customization requests can be submitted as an issue, like https://github.com/novatorem/novatorem/issues/2

If you want to share your own customization options, open a PR if it's done or open an issue if you want it implemented by someone else.

## Debugging

If you have issues setting up, try following this [guide](https://youtu.be/n6d4KHSKqGk?t=615).

Followed the guide and still having problems?
Try checking out the functions tab in vercel, linked as:
```https://vercel.com/{name}/spotify/{build}/functions``` 

<details><summary>Which looks like-</summary>

![image](https://user-images.githubusercontent.com/16753077/91338931-b0326680-e7a3-11ea-8178-5499e0e73250.png)

</details><br>

You will see a log there, and most issues can be resolved by ensuring you have the correct variables from setup.

