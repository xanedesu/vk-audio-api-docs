## audio.getRecomendations

Returns a list of suggested audio files based on a user's playlist or a particular audio file.

> This method can be called with a user token. [Access rights](https://vk.com/dev/permissions) required: **audio**.

### Parameters

<table>
  <tr>
    <td>
      <b>target_audio</b>
    </td>
    <td>
      Use to get recommendations based on a particular audio file. The ID of the user or community that owns an audio file and that audio file's ID, separated by an underscore.
      <blockquote>
        string
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>user_id</b>
    </td>
    <td>
      Use to get recommendations based on a user's playlist. User ID. By default, the current user ID.
      <blockquote>
        positive number
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
        positive number, maximum value <b>1000</b>, default <b>100</b>
      </blockquote>
    </td>
  </tr>
  <tr>
    <td>
      <b>shuffle</b>
    </td>
    <td>
      <i>1</i> — shuffle on
      <blockquote>
        flag, either <b>1</b> or <b>0</b>
      </blockquote>
    </td>
  </tr>
</table>

### Result

Returns the total results number in **count** field and an array of objects describing [audio](https://vk.com/dev/objects/audio) in <b>items</b> field.

> NOTE: Links to .mp3 files are bound to an IP address.

### Errors

<table>
  <tr>
    <td>
      <b>19</b>
    </td>
    <td>
      Content blocked
    </td>
  </tr>
</table>

Global errors can occur while running. See their descriptions on [this page](https://vk.com/dev/errors).