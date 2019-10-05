## audio.add

Copies an audio file to a user page or community page.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>audio_id</b>
    </td>
    <td>
      Audio file ID.
      <blockquote>
        positive number, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>owner_id</b>
    </td>
    <td>
      ID of the user or community that owns the audio file. Use a negative value to designate a community ID.
      <blockquote>
        int (number), <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>group_id</b>
    </td>
    <td>
      Community ID, needed when adding the audio file to a community (without minus).
      <blockquote>
        int (number)
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
        positive number
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the ID of the created audio file.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).