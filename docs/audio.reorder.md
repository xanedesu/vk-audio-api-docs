## audio.reorder

Reorders an audio file, placing it between other specified audio files.

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
  <tr>
    <td>
      <b>before</b>
    </td>
    <td>
      ID of the audio file before which to place the audio file.
      <blockquote>
        int (number)
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>after</b>
    </td>
    <td>
      ID of the audio file after which to place the audio file.
      <blockquote>
        int (number)
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns <i>1</i> if succeeded. 

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).