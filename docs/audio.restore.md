## audio.restore

description

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
      ID of the user or community that owns the audio file.
      <blockquote>
        int (number), current user id is used by default
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns an object descibing [audio](https://vk.com/dev/objects/audio). If audio storage time expires (usually it is 20 minutes), the server will throw **error 202 (Cache expired)**.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).