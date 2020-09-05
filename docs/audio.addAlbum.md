## audio.addAlbum

Creates an empty audio album.

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>group_id</b>
    </td>
    <td>
      Community ID (if the album will be created in a community).
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>title</b>
    </td>
    <td>
      Album title.
      <blockquote>
        string, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the ID of the created album.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
