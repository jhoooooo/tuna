---
layout: default
---
# Information

- Links:
  - https://discord.gg/e5DQ8yKnj6
  - https://twitter.com/jhooo_o
  - https://ko-fi.com/jhooo/shop

# How to install Tuna for Windows

1.  Determine your Windows system type by going to `[Settings > System > About > Device Specifications > System Type]`. It will say either "64-bit Operating System" or "32-bit Operating System".
2.  Download the Tuna plugin for OBS from the official [GitHub](https://github.com/univrsal/tuna/releases/latest) page.
    (Example: tuna-1.9.5-windows-x64-Installer.exe for "64-bit Operating System").
3.  Run the installer and follow it's instruction.
4.  Open OBS and go to the `[Tools > Plugins > Tuna Settings > Basics]`.
5.  Note.
    - The port number at `[Host/receive information on local webserver with port:]`.
    - The `[Refresh rate]`. Recommended *1000ms* or *500ms*.
    - Set the `[Song source]` as *Spotify*.

![](https://i.postimg.cc/3wt3sZ8y/obs64-Tg-Af-BCzm9z.png)

6.  Apply the changes.
7.  Switch to `[Spotify]` tab to the right of the window.
8.  Click on `[Open login page]`.
    
    > !! **DO NOT SHARE YOUR AUTH CODE**

9.  Copy your authentication code and paste it into the authentication field.
10. Click on `[Request token]`.
11. Apply the changes. Tuna settings is complete.
 (edited)

---

# How to setup the widget

1.  Download the widget from [ko-fi](https://ko-fi.com/jhooo/shop).
2.  Extract the downloaded ZIP file to a location of your choice.
3.  Now you can add new browser source on OBS.
   `[Sources > Browser > Create New > Name it > Select local file > Browse the location you extracted the zip earlier >
    choose Tuna_Spotify_widget_1.0_public.html > Set the width to "274" and height to "64" > ok.]`
4.  You won't see the widget if no song is playing.
5.  To setup the widget visual, go the location you extracted the zip, open the html file on your text editor such as notepad or [notepad++](https://notepad-plus-plus.org/downloads/).
6.  Scroll down and find `User Config` section[^1].

```javascript
    //SECTION ---------------->>>> User Config <<<<----------------

    const hide_cover = false;                       // show or hide albumcover entirely. [true/false]
    const album_cover_pulse = true;                 // Make album cover pulse. [true/false]
    const album_cover_pulse_color = '#f2baf1ba';    // Color of the pulse. Use 8 digits hex for transparency/opacity (or just add 'ba' at the end of 6 digit hex). ['#FFFFFFBA']
    const album_cover_circle = true;                // Make album circle [true/false]
    const album_cover_border_radius = '4px';        // if cover circle is 'false', it be square with this border radius size. ['number + px']
    const album_cover_spin = true;                  // Make album cover spin. [true/false]
    const music_player_background_style = 7;        // Widget background color, choose between [1 ~ 7]
    const tuna_server_port = 1608;                  // (1608) Number is located at : OBS > Tools > Tuna Settings [Host/receive information on local webserver with port]
    const tuna_refresh_rate = 500;                  // Number is located at : OBS > Tools > Tuna Settings [Refresh rate]

    //!SECTION ---------------->>>> User Config <<<<----------------
```

7.  You can change stuffs here and there is some explanation on what it does along side each settings.
8.  Ensure settings such as `tuna_server_port` & `tuna_refresh_rate` are the same as your tuna setting on OBS.
9.  You can also directly change other code there including the css, html and javascript directly.
10. If you need more help in general or to customize the widget, you can reach out at #help channel.

# Terms

The software product ("Product") relies on third-party services. While we make every effort to ensure that the Product works seamlessly with these services, we cannot guarantee their availability or reliability. We also cannot be held responsible for any changes to these services that may affect the Product's functionality.

By using the Product, you acknowledge and agree that:

The Product is provided "as is" and without any warranty or guarantee, either express or implied.
We will not be liable for any direct, indirect, incidental, consequential, special or punitive damages arising out of or in connection with the use of the Product.
You are solely responsible for your use of the Product and for ensuring that it complies with all applicable laws, regulations, and policies.
We recommend that you use the Product in a testing or development environment before deploying it in a production environment. If you choose to use the Product in a production environment, you do so at your own risk.

By using the Product, you also agree to indemnify and hold harmless the creators of the Product from and against any claims, actions, suits or proceedings, as well as any and all losses, liabilities, damages, costs and expenses (including reasonable attorneys' fees) arising out of or in connection with your use of the Product.

---

[^1]: Free version does not have this option.
