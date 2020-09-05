## audio.getAlbums

Returns a list of audio albums of a user or community.

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>owner_id</b>
    </td>
    <td>
      ID of the user or community that owns the audio file.
      <blockquote>
        int (number), current user id is used by default
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>offset</b>
    </td>
    <td>
      Offset needed to return a specific subset of albums.
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>count</b>
    </td>
    <td>
      Number of albums to return.
      <blockquote>
        positive number, maximum value <b>100</b>, default <b>50</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the total number of albums and an array of **album** objects, each containing the following fields: 
* **id** — Audio album owner ID;
* **owner_id** — Album ID;
*  **title** — Album title.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
