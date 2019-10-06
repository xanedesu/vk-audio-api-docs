## audio.get

Returns a list of audio files of a user or community.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>owner_id</b>
    </td>
    <td>
      ID of the user or community that owns the audio file. Use a negative value to designate a community ID.
      <blockquote>
        int (number), current user id is used by default
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>album_id</b>
    </td>
    <td>
      Audio album ID.
      <blockquote>
        int (number)
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>audio_ids</b>
    </td>
    <td>
      IDs of the audio files to return.
      <blockquote>
        list of comma-separated positive numbers
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>need_user</b>
    </td>
    <td>
      <i>1</i> — to return information about users who uploaded audio files.
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>offset</b>
    </td>
    <td>
      Offset needed to return a specific subset of audio files.
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
      Number of audio files to return.
      <blockquote>
        positive number
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the total results number in <b>count</b> field and an array of [objects describing audio](https://vk.com/dev/objects/audio) in <b>items</b> field.

> NOTE: Links to .mp3 files are bound to an IP address.

### Errors

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).