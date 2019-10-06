## audio.editAlbum

Edits the title of an audio album.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>group_id</b>
    </td>
    <td>
      ID of the community where the album is located.
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>album_id</b>
    </td>
    <td>
      Album ID.
      <blockquote>
        positive number, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>title</b>
    </td>
    <td>
      New album title.
      <blockquote>
        string, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

In case of success returns <i>1</i>. 

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).