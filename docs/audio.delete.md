## audio.delete

Deletes an audio file from a user page or community page.

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

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
      ID of the user or community that owns the audio file.
      <blockquote>
        int (number), <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns **1**.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
