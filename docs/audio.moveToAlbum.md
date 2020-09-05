## audio.moveToAlbum

Moves audio files to an album.

> This method can be called with a [user token](https://vk.com/dev/access_token). [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>group_id</b>
    </td>
    <td>
      ID of the community where the audio files are located. By default, current user ID.
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
      ID of the album to which the audio files will be moved.
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>audio_ids</b>
    </td>
    <td>
      IDs of the audio files to be moved.
      <blockquote>
        NOTE: An album can hold up to 1000 audio files.
      </blockquote>
      <blockquote>
        list of comma-separated positive numbers, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

In case of success returns <i>1</i>.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
