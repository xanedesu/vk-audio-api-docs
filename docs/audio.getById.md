## audio.getById

Returns information about audio files by their IDs.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>audios</b>
    </td>
    <td>
      Audio file IDs, in the following format: {owner_id}_{audio_id}.
      <blockquote>
        list comma-separated strings, <b>required parameter</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns a [list](http://vk.com/dev/list) of [audio](https://vk.com/dev/objects/audio) objects.

> NOTE: Links to .mp3 files are bound to an IP address.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).
